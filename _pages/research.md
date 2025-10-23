---
layout: page
permalink: /research/
title: research
description:
years: [2021, 2020]
nav: true
---

<div class="section_title">Publications</div>

<div class="publications">

<h2 class="year">2025</h2>
<!-- MULTIVARIATE -->
  <div class="row">
    <div class="col-sm-2 abbr">
      <span class="badge badge-info">preprint</span>
    </div>
    <div id="3" class="col-sm-8">
        <div class="title">A joint spatiotemporal model for multiple longitudinal markers and competing events</div>
        <div class="author">
          <em>J. Ortholand</em>, S. Durrleman, S. Tezenas Du Montcel 
        </div>
         <div class="book"><em>Arxiv</em></div>
      <div class="links">
        <a class="abstract btn btn-sm z-depth-0" role="button">
        Abs
        </a>
         <a href="https://arxiv.org/abs/2501.08960"   role="button" target="_blank">Article</a>
          <a href="https://gitlab.com/JulietteOrtholand/joint_multi"   role="button" target="_blank">Repository</a>
      </div>
      <div class="abstract hidden">
        <p>
          Non-terminal events can represent a meaningful change in a patient's life. Thus, better understanding and predicting their occurrence can bring valuable information to individuals. In a context where longitudinal markers could inform these events, joint models with competing risks have been developed. Their precision relies on a reference time for which disease onset is often used. Nevertheless, chronic diseases have no clear onset, making it difficult to define a precise reference time. We propose a Joint cause-specific Spatiotemporal model to overcome this limitation and to capture a shared latent process, a latent age (temporal aspect), associated with the ordering of the longitudinal outcomes (spatial aspect). First, we validated our model on simulated real-like data. Then, we benchmarked our model with a shared-random-effect joint model on real ALS data using the PRO-ACT dataset. Finally, to show how the model could be used for description tasks, we analysed the impact of sex and onset site on the progression of ALS as well as the initiation of Non-Invasive Ventilation. The Joint cause-specific spatiotemporal model achieved similar performance to the shared random effect joint model while capturing the latent disease age and the impact of the ordering of longitudinal outcomes on the occurrence of the events with fewer parameters. The application study confirmed existing results for the Longitudinal outcomes and showed how to interpret the model. The proposed approach by disentangling a temporal and a spatial aspect of the disease opens the perspective to capture meaningful change in future clinical trials.

          </p>
        </div>
    </div>
  </div>

  <!-- UNIVARIATE -->
  <div class="row">
    <div class="col-sm-2 abbr">
      <span class="badge badge-secondary">proceedings</span>
    </div>
    <div id="3" class="col-sm-8">
        <div class="title">Joint model with latent disease age: overcoming the need for reference time</div>
        <div class="author">
          <em>J. Ortholand</em>, N. Gensollen, S. Durrleman, S. Tezenas Du Montcel 
        </div>
         <div class="book"><em>Accepted in Statistical Methods in Medical Research</em></div>
      <div class="links">
        <a class="abstract btn btn-sm z-depth-0" role="button">
        Abs
        </a>
        <a href="https://arxiv.org/abs/2401.17249"   role="button" target="_blank">Article</a>
        <a href="https://gitlab.com/JulietteOrtholand/jm_article"   role="button" target="_blank">Repository</a>
      </div>
      <div class="abstract hidden">
        <p>
          Heterogeneity of the progression of neurodegenerative diseases is one of the main challenges faced in developing therapies. Thanks to the increasing number of clinical databases, progression models have allowed a better understanding of this heterogeneity. Joint models have proven their effectiveness by combining longitudinal and survival data. Nevertheless, they require a reference time, which is ill-defined for neurodegenerative diseases, where biological underlying processes start before the first symptoms.

In this work, we propose a joint non-linear mixed-effect model with a latent disease age, to overcome this need for a precise reference time.

We used a longitudinal model with a latent disease age as a longitudinal sub-model. We associated it with a survival sub-model that estimates a Weibull distribution from the latent disease age. We validated our model on simulated data and benchmarked it with a state-of-the-art joint model on data from patients with Amyotrophic Lateral Sclerosis(ALS). Finally, we showed how the model could be used to describe ALS heterogeneity.

Our model got significantly better results than the state-of-the-art joint model for absolute bias on ALSFRS revised score (4.21(SD 4.41) versus 4.24(SD 4.14)(p-value=1.4e-17)), and mean-cumulative-AUC for right-censored events on death (0.67(0.07) versus 0.61(0.09)(p-value=1.7e-03)).

To conclude, we propose a new model better suited in the context of unreliable reference time.

          </p>
        </div>
    </div>
  </div>


  <!-- #2023 -->
  <h2 class="year">2023</h2>

  <!-- ALS -->
  <div class="row">
    <div class="col-sm-2 abbr">
      <span class="badge badge-success">journal</span>
    </div>
    <div id="3" class="col-sm-8">
        <div class="title">Interaction of sex and onset site on the disease trajectory of Amyotrophic Lateral Sclerosis</div>
        <div class="author">
          <em>J. Ortholand</em>, P.-F. Pradat, S. Durrleman, S. Tezenas Du Montcel 
        </div>
         <div class="book"><em>Journal of Neurology.</em></div>
      <div class="links">
        <a class="abstract btn btn-sm z-depth-0" role="button">
        Abs
        </a>
        <a href="https://link.springer.com/article/10.1007/s00415-023-11932-7"   role="button" target="_blank">Article</a>
         <a href="https://gitlab.com/JulietteOrtholand/als_sex_subtype_article"   role="button" target="_blank">Repository</a>
      </div>
      <div class="abstract hidden">
        <p>
          Background: Studies showed the impact of sex and onset site (spinal or bulbar) on disease onset and survival in ALS. However, they mainly result from cross-sectional or survival analysis, and the interaction of sex and onset site on the different proxies of disease trajectory has not been fully investigated. 
Methods: We selected all patients with repeated observations in the PRO-ACT database. We divided them into four groups depending on their sex and onset site. We estimated a multivariate disease progression model, named ALS Course Map, to investigate the combined temporal changes of the four sub-scores of the revised ALS Functional Rating Scale (ALSFRSr), the forced vital capacity (FVC), and the body mass index (BMI). We then compared the progression rate, the estimated age at onset, and the relative progression of the outcomes across each group.
Results: We included 1,438 patients from the PRO-ACT database. They were 51% men with spinal onset, 12% men with bulbar onset, 26% women with spinal onset, and 11% women with bulbar onset. We showed a significant influence of both sex and onset site on the ALSFRSr progression. The BMI decreased 8.9 months earlier (95% CI = [3.9, 13.8]) in women than men, after correction for the onset site. Among patients with bulbar onset, FVC was impaired 2.6 months earlier (95% CI = [0.6, 4.6]) in women. 
Conclusion: Using a multivariable disease modelling approach, we showed that sex and onset site are important drivers of the progression of motor function, BMI, and FVC decline. 
          </p>
        </div>
    </div>
  </div>


  <!-- AD -->
  <div class="row">
    <div class="col-sm-2 abbr">
      <span class="badge badge-success">journal</span>
    </div>
    <div id="3" class="col-sm-8">
        <div class="title">Forecasting individual progression trajectories in Alzheimer’s disease</div>
        <div class="author">
          E. Maheux, I. Koval, <em>J. Ortholand</em>, C. Birkenbihl, D. Archetti, V. Bouteloup, S. Epelbaum, C. Dufouil, M. Hofmann-Apitius, S. Durrleman
        </div>
         <div class="book"><em>Nature Communications.</em></div>
      <div class="links">
        <a class="abstract btn btn-sm z-depth-0" role="button">
        Abs
        </a>
        <a href="https://www.nature.com/articles/s41467-022-35712-5"   role="button" target="_blank">Article</a>
      </div>
      <div class="abstract hidden">
        <p>
          The anticipation of progression of Alzheimer’s disease (AD) is crucial for evaluations of secondary prevention measures thought to modify the disease trajectory. However, it is difficult to forecast the natural progression of AD, notably because several functions decline at different ages and different rates in different patients. We evaluate here AD Course Map, a statistical model predicting the progression of neuropsychological assessments and imaging biomarkers for a patient from current medical and radiological data at early disease stages. We tested the method on more than 96,000 cases, with a pool of more than 4,600 patients from four continents. We measured the accuracy of the method for selecting participants displaying a progression of clinical endpoints during a hypothetical trial. We show that enriching the population with the predicted progressors decreases the required sample size by 38% to 50%, depending on trial duration, outcome, and targeted disease stage, from asymptomatic individuals at risk of AD to subjects with early and mild AD. We show that the method introduces no biases regarding sex or geographic locations and is robust to missing data. It performs best at the earliest stages of disease and is therefore highly suitable for use in prevention trials.
          </p>
      </div>
    </div>
  </div>
