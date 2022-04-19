* Questions
  * why control group also have more 14 free days?
    * Also trt in control group, want to see if the Asthma-PASS 
    * time influence? 
    * missing?
  * 
  * Hypothesis: inferiority - study design

* Non-inferiority
  * A study that tests whether a new treatment is not worse than an active treatment it is being compared to.

# Analyze pilot study

* Data exploration

  * Intra-class correlation heatmap
  * spaghetti plot over trt~school
    * Time: continuous and categorical comparison?

* GLMM
  $$
  \begin{aligned}
  \log\frac{\pi_{ijk}}{1-\pi_{ijk}}&=\beta_0\\
  &+\beta_1t_{ijk}\\
  &+\beta_2I(\text{trt}=1)_i\\
  &+\beta_3I(\text{school}=2)_{ij}\\
  &+\beta_4I(\text{school}=3)_{ij}\\
  &+\beta_5I(\text{school}=4)_{ij}\\
  &+\beta_6I(\text{trt}=1)_{ij}\times t_{ijk}\\
  &+\gamma_{0i}+\gamma_{0j}\\
  &+\epsilon_{ijk}
  \end{aligned}
  $$
  

