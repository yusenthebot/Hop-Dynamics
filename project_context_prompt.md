# Project Context Prompt (prefix for poster-generation prompts)

Paste this block at the top of any prompt that asks an assistant to help design, edit, or render the poster. It gives the model everything it needs to reason about the project without re-reading the full proposal.

---

## PROJECT CONTEXT — read this before doing anything else

**Course & team.** CMU 24-775 *Bio-Inspired Robot Design* (Spring 2026), semester project. Team of 5: Yusen Xie (controls), Yutao Deng (mechatronics, motor dynamics), Zongyu Gao (hardware + soft-material simulation), Xinxuan Tang (CAD, stress/dynamics sim), Zijian Wang (mechatronics, actuator design, microcontroller).

**Project title.** *Bio-Inspired Wheeled-Biped Robot with Active Tail for Enhanced Terrain Traversal.*

**One-sentence pitch.** We are building a hybrid wheeled–bipedal robot with an actively actuated 2-DOF tail that uses tail-generated angular momentum as a functional tool — not just for passive balance — to cross gaps, climb steps, and traverse rough terrain that defeat a tail-less baseline.

**Biological inspiration.**
- **Kangaroo (primary):** tail acts as a dynamic inertial regulator and a third support limb during pentapedal locomotion; redistributes angular momentum to stabilize posture and contribute propulsion on uneven terrain (O'Connor et al., *Biology Letters* 2014).
- **Lizard (secondary):** tail-assisted pitch control — lizards modulate tail inertia mid-air to stabilize body pitch (Libby et al., *Nature* 2012). This is the theoretical basis for our active-tail control law.
- **Prior robots referenced:** kangaroo-hopping robot with active tail (Liu 2014), Penn KodLab tails-for-dynamic-balance, Ascento two-wheeled jumping robot (ETH 2019, no tail), IROS 2015 tail-assisted legged leaping.

**Research gap we address.** Existing wheel-foot hybrids either ignore tails or use them passively (stair support, mid-air pitch only). No one has integrated an actively controlled tail that simultaneously (a) redistributes angular momentum for pitch stabilization AND (b) serves as a third ground contact during obstacle negotiation on a wheeled-biped platform.

**Core hypothesis.** A tailed wheeled-biped maintains stable locomotion (pitch std. dev. σ < 5°, ≥80% traverse success) across terrain whose surface roughness Ra is **40–50% higher** than the tail-less baseline's limit.

**System overview.**
- **Morphology:** two-wheeled biped body with two driven wheels + a 2-DOF active tail terminated by a tip mass to boost inertia.
- **Two operating modes, state-machine switched:**
  1. **Static Tripod Mode** — robot sits on two wheels + tail tip (low-energy, stable).
  2. **Dynamic Balancing Mode** — active tail applies counter-torque for pitch stabilization while the robot rolls (agile, active balance).
- **Three candidate tail architectures under evaluation:** (1) rigid-link series driven by high-speed servos; (2) pneumatic-rigid hybrid for high power-to-weight impulse; (3) multi-chamber soft-silicone inflation tail for variable stiffness and impact resilience.
- **Build stack:** 3D-printed PLA / TPU / silicone parts, carbon-fiber rod reinforcement, BLDC motors (2 wheels + 2 leg joints + 1 tail joint), ESCs, LiPo pack, IMU, MCU. Budget ~$531.
- **Simulation tools:** MATLAB/Simulink and/or PyBullet for controller validation before hardware.

**Experimental plan (uneven terrain traversal).**
- **Independent variables:** tail configuration {Active, Locked, None}; terrain roughness Ra ∈ {5, 10, 15, 20, 25 mm} via 3D-printed/laser-cut tiles.
- **Dependent variables:** pitch standard deviation σ from onboard IMU (OptiTrack ground truth optional), success rate (% of trials completing the ~2 m track without falling or intervention).
- **Protocol:** constant ~0.4 m/s forward command, N ≈ 10 trials per condition.
- **Success criteria:** σ < 5° and success rate ≥ 80% per Ra level; report max traversable Ra per tail config; target improvement (Ra_tail − Ra_baseline) / Ra_baseline × 100 ≈ 40–50%.

**Stretch goal.** Closed-loop dynamic control architecture that decouples attitude stabilization from propulsion — counteracting acceleration-induced pitch during high-speed rolling and autonomously regulating mid-air body orientation via angular-momentum transfer for recoverable landings after ballistic hops.

**Impact / applications.** Search-and-rescue, remote inspection, exploration in unstructured environments where legged-only robots are slow and wheeled-only robots fail on discontinuous terrain.

**Key visuals available for the poster.**
- Kangaroo reference photos (fighting stance, pentapedal tail kinematics).
- CAD renders of the wheeled-biped assembly (by Zijian) and the 2-DOF active tail with tip mass (by Yusen).
- Concept sketches: pneumatic soft-tail stair-climbing (Gao), underactuated spine-like multi-link tail (Xinxuan), rigid swinging tail for inertial assist (Yutao).
- Conceptual illustration of the **Static Tripod ↔ Dynamic Balancing** mode-switch state machine.
- Gantt chart (3 phases over 9 weeks).
- Planned plots: pitch σ vs. Ra for each tail configuration; success rate vs. Ra bar chart; Max-Ra-traversed comparison; photos/video stills of the physical experiment.

**Tone & audience.** This is a mid-semester / onsite-review poster for a graduate engineering audience. Keep language technical but crisp. The key takeaway the reader must leave with: *"An actively controlled bio-inspired tail lets a wheeled-biped traverse ~40–50% rougher terrain than a tail-less baseline, by acting as both an inertial stabilizer and a third ground contact."*
