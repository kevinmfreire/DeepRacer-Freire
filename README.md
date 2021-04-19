# Reinforcement Learning Project
Project Link Video
https://www.loom.com/share/d43b6fdd0484491888623e51a909fce9
## Self Driving autonomous Race car

This source code was taken and intensilve modified from AWS jail broken version.  Please Read ./DEFAULT_INFO.md to get default information about this code.

This README file is to showcase some of the modifcations we did to get our project going and running.

## The main notebook instance we ran was

    ./deepracer_rl.ipynb

This notebook contained all our setup and code to get our project running.  Most of it was mofied based on existing AWS code.

modified directories

custom rewards function can be found in

    ./src/artifacts/rewards/andrei_reward_optimized_turns.py

custom action space config can be found in

    ./src/artifacts/actions/freire_continous_custom_architecture.json

custom architecture code lines 80-89 (called DEEP_CONVOLUTIONAL_NETWORK_FREIRE)

    ./src/markov/sensors/utils.py

final latex report files can be found in

    ./report

Videos of a sample training and testing session can be found in

    ./videos


Finally, this source code had to be heavily modifed for it to work with our requirements.  This included capabilites to execute PPO Continuos algorithm becase the default code only allowed SAC (please see issue #2055 in https://github.com/aws/amazon-sagemaker-examples/tree/master/reinforcement_learning/rl_deepracer_robomaker_coach_gazebo).

we customized the ./src/markov/ directory build to allow the use of our own architecture for research purpose.

Thanks to AWS we were able to complete such a large project in such a short time!

## Model
Our models were too big in size to submit over 3 GB and we could not upload it to our github repo because github has size restriction.  If you want to see our model email us and we can try to give you access to our S3 bucket to download.
We used AWS S3 data storage buckets to store our data and fetch it because keeping a notebook running for months was so expensive that this was our only option.

Trying to run this notebook will fail unless you configure it to match your AWS account.  If you wish to run this please message developers


Walter Freire and Kevin Freire

Walter : andrei.freire@ryerson.ca

Kevin  : kfreirea@ryerson.ca

