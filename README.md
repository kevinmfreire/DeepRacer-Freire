# Reinforcement Learning Project

## Self Driving autonomous Race car

This source code was taken and intensilve modified from AWS jail broken version.  Please Read ./DEFAULT_INFO.md to get default information about this code.

This README file is to showcase some of the modifcations we did to get our project going and running.

modified directories 

custom rewards function can be found in 

    ./src/artifacts/rewards/andrei_reward_optimized_turns.py
    
custom action space config can be found in
    
    ./src/artifacts/actions/freire_continous_custom_architecture.json
    
custom architecture code lines 80-89 (called DEEP_CONVOLUTIONAL_NETWORK_FREIRE)
    
    ./src/markov/sensors/utils.py
    
## The main notebook instance we ran was

    ./deepracer_rl.ipynb 
    
This notebook contained all our setup and code to get our project running.  Most of it was mofied based on existing AWS code.



Finally, this source code had to be heavily modifed for it to work with our requirements.  This included capabilites to execute PPO Continuos algorithm becase the default code only allowed SAC (please see issue #2055 in https://github.com/aws/amazon-sagemaker-examples/tree/master/reinforcement_learning/rl_deepracer_robomaker_coach_gazebo).

we customized the ./src/markov/ directory build to allow the use of our own architecture for research purpose. 

Thanks to AWS we were able to complete such a large project in such a short time!

## Model

In the directory
    ./models
We added our latest model that we trained for 8 hours.  We used S3 buckets to store our data and fetch it because keeping a notebook running for months was so expensive that this was our only option.  
Trying to run this notebook will fail unless you configure it to match your AWS account.  If you wish to run this please message developers


Walter Freire and Kevin Freire

Walter : andrei.freire@ryerson.ca

Kevin  : kfreirea@ryerson.ca

