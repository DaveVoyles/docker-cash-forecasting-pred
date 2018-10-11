
# Docker container running a flask web server for cash flow prediction using Scikit-Learn

#### Author(s): MSFT Commercial Software Engineering 

Create a docker container and host it in Azure with this tutorial
----------
### Why would you want to use this?
Imagine that you have built a machine learning model and want others to be able to use it. You'd have to host it somewhere, and as more users hit the endpoint with the model, you'll need to scale dynamically to assure they have a fast and consistent experience. This project includes a number of simple, yet helpful tools.

**Docker**

Docker is a platform that allows users to easily pack, distribute, and manage applications within containers. It's an open-source project that automates the deployment of applications inside software containers. Gone are the days of an IT professional saying  "*Well, it worked on my machine.*" Not it works on all of our machines.

**Flask**

Flask is great for developers working on small projects that need a quick way to make a simple, Python-powered web site. It powers loads of small one-off tools, or simple web interfaces built over existing APIs.

**Scikit-Learn**

Scikit-Learn is a simple and efficient tools for data mining and data analysis, which is built on NumPy, SciPy, and matplotlib. It does a lot of the dirty work involved with machine learning, and allows you to quickly build models, make predicitons, and manage your data.

Once your docker container is deployed, you simply make an HTTP Post request to ```<YourWebsite>:5000/prediction``` with the csv of an dataset in the body, and the model will return a prediction for cash on hand.
