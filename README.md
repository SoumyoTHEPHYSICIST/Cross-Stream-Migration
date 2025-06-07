# Cross-Stream-Migration
# 🌀 Cross-Stream Migration of a Rigid Sphere in 2D Poiseuille Flow

Hey there! 👋  
This project dives into the fascinating world of how tiny particles (rigid spheres) move sideways (cross-stream) in a fluid flowing between two plates — specifically in **viscoelastic (non-Newtonian) fluids**.

We explore different types of motion:
- **Inertial migration** (in Newtonian fluids)
- **Viscoelastic migration**
- **Electrophoresis-enhanced migration**
- **Forced migration** (sedimentation)

Let’s break things down 👇

---

## 🚀 The Big Idea

Normally, particles in low Reynolds number flows just go with the flow. But real life isn’t always that simple — sometimes they move sideways across streamlines. This lateral migration can happen due to:
- Inertia (in Newtonian fluids)
- Normal stress differences (in non-Newtonian fluids)
- External forces like gravity or electric fields

And that’s what this work is all about.

---

## 🔍 Topics Covered

### 1. **Inertial Migration (Newtonian Fluid)**  
- At very low inertia (Re → 0), particles don’t migrate laterally.
- But experiments show migration happens → enter the **Segre-Silberberg effect**.
- Using asymptotic expansions and the **Lorentz Reciprocal Theorem**, we estimate the lift force due to inertia.
- Force is weak (~Re·κ²), but it's there.

---

### 2. **Viscoelastic Migration**  
- Second-order (polymer-like) fluids behave differently.
- Even without inertia, **normal stress differences** push particles toward the flow centerline.
- Lift force here is ~λ·κ³ — stronger than in Newtonian case.
- The stress field near the particle is the main player (not the walls).

---

### 3. **Electrokinetically Enhanced Migration**  
- Add an electric field? Boom — huge change!
- Particle develops a slip velocity at the surface (due to zeta potential).
- Result: a much stronger lateral force (~order 1).
- Migration direction flips compared to sedimentation (gravity-driven) case.
- Super helpful for microfluidics and lab-on-chip setups!

---

### 4. **Sedimentation (Forced Migration)**  
- A non-neutrally buoyant particle (heavier/lighter than the fluid) sediments.
- This creates a disturbance field dominated by a **Stokeslet**, not a source dipole like in electrophoresis.
- Result: stronger lateral migration, but in a different direction than the electrophoretic case.

---

## 📈 Particle Trajectories

We didn’t stop at theory — we tracked how these particles actually move!

- **In viscoelastic flow**, particles slowly drift to the center.
- **Electrophoretic particles** migrate faster (thanks to that slip).
- **Sedimenting particles** show a sharper curve but go in the opposite direction.

Used simple explicit Euler method to plot trajectories:
- Position vs time
- Position vs axial flow

---

## 🧠 Cool Observations

- The **lift force** from electrophoresis is stronger than viscoelastic migration alone.
- In sedimentation, the **buoyancy number (B)** is the big influencer.
- In viscoelastic migration, wall effects are tiny — it’s all about local stresses near the particle.
- **Opposite behavior**: Electrophoresis pulls you in, sedimentation pushes you out.

---

## 🛠 How We Did It

- **Asymptotic expansion** of velocity and stress fields
- Used **Lamb’s general solution** for reflections
- Applied the **Lorentz Reciprocal Theorem (LRT)** to compute forces without solving full velocity fields

---

## 🔮 What's Next?

Some future directions we’re working on:
- Derive full first-order velocity fields and compare lift from both LRT and direct integration
- Clarify tricky derivations from Peery’s and Ganesh Subramanian’s papers
- Better understand inertia’s role in the particle’s migration in complex fluids

---

## 📚 References

- Choudhary et al., *J. Fluid Mech.*, 2019 & 2020  
- Ho & Leal, *J. Fluid Mech.*, 1976  
- Guazzelli & Morris, *A Physical Introduction to Suspension Dynamics*

---

## ✍️ Author

**Soumyodeep Chowdhury**  
- soumyodeep24@iitk.ac.in

---

