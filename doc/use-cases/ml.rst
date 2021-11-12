Machine Learning
================

Ploomber has many features specifically tailored to accelerate Machine Learning
workflows. For instance, it makes the cleaning and the feature engineering
development process more manageable since it allows you to break down logic
in small steps. Furthermore, you can quickly deploy models in batch or
online mode.


Data cleaning and feature engineering
*************************************

Data cleaning and feature engineering are highly iterative processes, Ploomber
accelerates them via :ref:`incremental builds <incremental-builds>`, which allow
you to introduce changes to your pipeline and bring results up-to-date without
having to re-compute everything from scratch.

Experiment tracking
*******************

Ploomber also plays nicely with experiment
trackers, `here's an example <https://github.com/ploomber/projects/tree/master/templates/mlflow>`_
showing how to integrate Ploomber with MLflow.

Parallel experiments
********************

To help you find the best performing model, Ploomber allows you to parallelize
Machine Learning experiments. If you're using the Spec API (``pipeline.yaml``),
you can use the :doc:`grid feature  <../cookbook/grid>` to create many tasks
at once with different parameters. If you're using the Python API, you can
easily create highly customized grids of tasks.

Large-scale model training
**************************

If one machine isn't enough, you can parallelize training jobs in a cluster
by :doc:`exporting your pipeline <../deployment/large-scale-training>` to any
of our supported platforms (Kubernetes, Airflow, and AWS Batch).


Deployment
**********

Once you find the best performing model, you can deploy it
for :doc:`batch processing <../deployment/batch>` or as
an :doc:`online API <../deployment/online>`.



