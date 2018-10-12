EARTHQUAKE PREDICTION AND MANAGEMENT SYSTEM

Earthquakes have often been the harbinger of mass destruction.

PREDICTION 

DATASET

Seismographs

Seismographs can detect quakes that are too small for humans to feel. During an earthquake, ground-shaking seismic waves radiate outward from the quake source, called the epicenter.

Different types of seismic waves travel at different speeds and through different parts of the Earth during a quake.

The farther seismic waves get from their source, the weaker they become. A network of interconnected seismographs can quickly pinpoint the source of a quake by measuring differences in the time it takes different seismic waves to reach a detector.

Because seismographs can only measure movement in one direction, many seismograph stations have multiple seismographs to record the north-south, east-west, and vertical motions of the ground.

The prediction model uses seismograph data captured from live data streamed on http://quakes.world/live-seismograph/ . 

Time series Data

Time series data is data which depends on time i.e. it has relationship with the time step before it. 

Earthquakes carry information in the form of seismic waves(having a temporal relationship) which contain data in the form of records. In order to capture this important piece of information into our model we take this data and use it in LSTM network. 

In addition to this some other sources have been used to collect data from seismographs i.e. http://ds.iris.edu/ds/nodes/dmc/software/downloads/irisfetch.m/ and https://www.researchgate.net/publication/323992824_A_spectrum-based_adaptive_sampling_algorithm_for_smart_sensing#pfc.

MODEL USED

The prediction model is based on LSTM neural network(on time series datapoints) along with CNN on data images(seismographs) and then combines the trained model to get a prediction.

MANAGEMENT SYSTEM

Machine Learning Algorithms are not 100% accurate although they have high probabilities to detect or predict things. In order to predict things, we will use the model mentioned above.

However, In case of a misprediction, it becomes evident to put a management system in place to take care of any contigencies.
The management system we propose is to create a region-wise Disaster-Aid-Relief System based on data gathered from Sources.

The application uses GoogleMaps to point out specific regions which are in need of Disaster-Relief.

It captures the spending of money on the Relief-Measures as well as the next best possible investment.

It uses economic measures such as opportunity cost and certain other metrics e.g. Relief-Aid/(no. of people * distance from base) to model this management system.
