# Assignment 1: Setup & Debugging Journal
**MLOps & ML Programming (2026)**

## Student Information
* **Name:** `[Nizaar Cherdud Amri]`
* **Student ID:** [1778118]
* **TA Name:** `[Darius Barsony]`
* **GitHub Repository:** [Link to your repository]
* **Base Skeleton Used:** [https://github.com/SURF-ML/MLOps_2026/tree/main](https://github.com/SURF-ML/MLOps_2026/tree/main)

---
Example including an image:
![PCAM](assets/pcam.jpg)
---

## Question 1: First Contact with Snellius
1. **Connection Details:**
   - **Command:** `[ssh scux2259@snellius.surf.nl]`
   - **Login Node:**  `[int5]`
   - **Screenshot:** `[link]`

2. **Issues Encountered:**
   - **Error Message:** `[Only misstyped password: no error message]`
   - **Resolution:** `[Typing proper password]`

3. **Smooth Connection (If applicable):**
   - **SSH Client:** [e.g., OpenSSH v9.2]
   - **Prior Experience:** `Webtech Project requirde ssh use for git`
   - **Preemptive Steps:** `[None]`

---

## Question 2: Environment Setup
1. **Setup Sequence:**
   - **Commands:** [Paste output of history]
   - **Full Venv Path:** `[Paste output of realpath]`

2. **Pip Install Torch:**
   - **Duration:** [Approximate time]
   - **Warnings:** [Warnings about pip version/dependencies]
   - **Venv Size:** `[Paste output of du -sh]`

3. **Mistakes/Unexpected Behavior:**

4. **Verification:**
   - **Output:** `[Paste output of python -c command]`
   - **Explanation:** [Why is CUDA False on a login node?]

---

## Question 3: Version Control Setup
1. **GitHub URL:** [Link]
2. **Authentication:** [HTTPS/SSH/CLI] + [Errors encountered]
3. **.gitignore:**
   - **Contents:** [Paste code block]
   - **Important items to include:** [Reasoning]
   - **README info:** [Should Snellius access info be in README?]
4. **Git Log:** `[Paste output of git log --oneline]`

---

## Question 4: Your First Batch Job (Slurm)
1. **Files Provided:** [List your .sh, .py, and output.txt files included in zip]
2. **Job ID & Stats:** `[Paste output of sacct command]`
3. **Submission Problem:** [Describe error and diagnosis]
4. **Verification:** [Proof that script ran successfully]
5. **Login vs Batch:** [Explain the difference]
6. **Why Clusters?:** 
---

## Question 5: Reflection & Conceptual Understanding
1. **The Filesystem:**
   - **I/O Performance:** [Why 100k small files are bad]
   - **Mitigation Strategies:** [Strategy 1] and [Strategy 2]
   - **Dataset Versioning:** [How to handle GB/PB datasets]
2. **Reproducibility:** [3 specific causes of different results + MLOps fixes]
3. **Conda vs venv vs uv:** [Pros/Cons of each for Snellius]

---

## Question 6: Package Integrity
1. **ModuleNotFoundError:** [Describe any PYTHONPATH or __init__.py issues]
2. **Import Abstraction:** [Why import from ml_core.data vs ml_core.data.pcam?]
3. **Pytest Result:** `[Paste output of pytest tests/test_imports.py]`

---

## Question 7: The Data Pipeline
1. **Implementation:** `[Paste __getitem__ method]`
2. **Local Pytest:** `[Paste output of pytest tests/test_pcam_pipeline.py]`
3. **CI Pipeline:**
   - **Screenshot:** ![GitHub Actions Tab](assets/github_actions.png)
   - **Reflection:** [CI vs Local discrepancies]
4. **Sampling Math:** [Average positives with vs without WeightedRandomSampler]
5. **EDA Plots:**
   - ![PCAM Intensity Outliers](assets/pcam.png)
   - [Additional plots as requested]

---

## Question 8: Model Implementation (MLP)
1. **Forward Pass:** [Error details + dimension calculation for (3, 96, 96)]
2. **Weight Updates:** [Why check backprop explicitly?]
3. **Test Output:** `[Paste output of pytest on the relevant file]`

---

## Question 9: Training Loop & Loss Visualization
1. **Training Execution:** [Method used + Node ID (gcnXX)]
2. **Loss Visualization:**
   - **Plot:** ![Training and Validation Loss](assets/loss_plot.png)
   - **Trajectory Analysis:** [Healthy curve? Trajectory hypothesis?]
3. **Most Frustrating Error:**
   - **Error Message:** `[Traceback]`
   - **Debugging Steps:** [How you resolved it]

---

## Final Submission Checklist
- [ ] Folder contains .md file and assets/ folder?
- [ ] Name and Student ID on page 1?
- [ ] All code/terminal snippets are in backtick blocks?
- [ ] All images use relative paths (e.g., assets/pcam.png)?
- [ ] Slurm .sh and .out files included in the .zip?