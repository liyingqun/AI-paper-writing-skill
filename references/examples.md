# Preferred Writing Examples

These are structural examples, not research evidence. Any symbolic result labels must be replaced with the researcher's verified information before publication.

## Observation-driven motivation

Weak:

> Deep learning has recently achieved remarkable progress. We therefore propose a novel consistency framework.

Preferred, when documented by the study:

> We observed that different perturbations of the same image produced different predictions. This observation motivates the question of how to maintain prediction consistency across perturbed inputs. We address this question by introducing a consistency objective during training.

## Method instead of operational instructions

Operational content for the linked GitHub README:

> Execute the training script and set the consistency-weight argument.

Scientific description, when this is the actual method:

> To align predictions across paired views of an input, we optimize a joint classification and consistency objective:
> 
> \[
> \mathcal{L}(\theta)=\mathcal{L}_{\mathrm{cls}}(\theta)+\lambda\mathcal{L}_{\mathrm{cons}}(\theta).
> \]
> Here, \(\theta\) denotes the trainable parameters, \(\mathcal{L}_{\mathrm{cls}}\) is the classification loss, and \(\mathcal{L}_{\mathrm{cons}}\) measures disagreement between predictions for paired views. The coefficient \(\lambda\) sets the relative weight of consistency training.

The complete Method must define the actual losses, paired-view construction, and optimization procedure used in the research.

## Direct framing

Defensive:

> Although the architecture is simple, it still has scientific value.

Direct:

> The architecture integrates information from multiple feature sources through learned weights.

Defensive:

> Despite using only two datasets, our experiments still demonstrate effectiveness.

Direct:

> We use datasets A and B to evaluate classification under two data distributions.

Defensive:

> This study is not intended to address every possible setting.

Direct:

> This study addresses image classification under a fixed computational budget.

## Contribution versus activity

Activity:

> We conduct extensive experiments and analyze different parameters.

Contribution structure:

> We introduce [specific mechanism] to address [specific research problem].

Replace the bracketed fields with established research content. Add a separate empirical finding when it is a distinct contribution supported by the experiments.

## Objective related work

Preferred structure:

> Study A addresses cross-domain recognition through feature alignment. Study B incorporates class information into the alignment objective. Study C combines this direction with self-supervised representation learning.

Use real studies, verified descriptions, and citations in the manuscript.

## Question-driven experiment

Weak:

> We also conduct an ablation study.

Preferred:

> To measure the contribution of the consistency objective, we compare the complete model with a variant trained without that objective. Both variants use the same backbone, data split, and training schedule.

## Interpretation beyond table narration

Table narration:

> Model A has score a, model B has score b, and the complete model has score c.

Interpretive structure:

> Adding the consistency objective changes [named metric] from [verified baseline value] to [verified full-model value]. Across the tested perturbation levels, [documented trend]. These results answer [experimental question] by showing [specific finding].

## Concrete conclusion and future direction

Use the study's research question, defining design, selected verified measurements, and resulting finding. State a specific next research task, such as evaluating the same mechanism under a new data distribution or extending the formulation to a defined task. Replace generic closing phrases with the actual development proposed by the researcher.
