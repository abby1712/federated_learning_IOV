# Intrusion Detection Models on Internet of vehicles by Federated learning.

Federated learning is a method of training machine learning models in which data is distributed across multiple devices or locations, rather than being centralized in a single location. Each device, or "edge" device, trains a local version of the model using its own data, and then periodically sends updates to a central server, which aggregates the updates to improve the overall model. This allows for models to be trained on a much larger and more diverse dataset, and also helps to protect the privacy of users by keeping their data on their own devices.

The following is a detailed workflow of the Federated Learning process:

Data Partitioning: The data is divided and distributed among the edge devices. Each edge device has a local dataset that it can use to train its own model.

Initial Model Training: The edge devices use their local datasets to train a local model. This is done independently of the other edge devices and the central server.

Model Update: After the edge devices have trained their local models, they send the updated model parameters to the central server.

Model Aggregation: The central server receives the updated model parameters from the edge devices and aggregates them to create a new global model. This can be done by taking the average of the updates or by using other techniques such as weight averaging or voting.

Model Broadcast: The central server sends the new global model back to the edge devices.

Evaluation: The updated global model is evaluated using a test dataset, the accuracy is calculated as an evaluation metric.

Repeat: The edge devices use the updated global model to retrain their local models and the process repeats from step 3.

Termination: The process terminates when the global model has converged or the desired accuracy is achieved.
