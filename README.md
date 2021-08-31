# DevOps Exercise
take-home project for the DevOps interview.


## Goal

Implement a small Kubernetes cluster with multiple services communicating to each other in a load-balanced way.


## Requirements

Create the following Kubernetes services on Google Cloud Platform:

1. Create a service (users) with a single endpoint that returns a user name when given a user_id (e.g., GET `/users/1234`). The user name can be randomly generated, doesn't have to actually come from a database.

1. Create another service (countries) with a single endpoint that, when given a user id, returns the user's name and country (e.g., GET `/countries?user_id=1234`). The countries service should issue a request to the users service to get the user's name. The country can also be randomly generated; it doesn't have to come from a database.

The users service(2 pods) should be independently able to scale from the countries service(3 pods). Request from the countries service should be sent to the users service in a load-balanced way. The countries service is the only service that is visible to the internet. Make sure all the requests are getting logged in the log explorer.

You can use any language to create underlying web servers. You can use as many open source libraries or packages as needed.


## Process

There's no deadline, but please spend no more than an hour or so on this exercise. In the interest of keeping it untimed, please take as much time as you need and book something [here](https://calendly.com/bk42/90min) when you think you'd be ready. It might be helpful to fork this repo and add your code to it so that our team can take a look before we talk. If you have reservations about making your code public, feel free to keep your fork private and give us admin access to bk (at) abstractops.com, so that I can add other folks as needed.

You should have received an invite to a separate empty project in our GCP for this task.

If you have any questions/concerns, feel free to email me at bk (at) abstractops.com. Thank you for taking the time to work on this, genuinely appreciate it 🙏
