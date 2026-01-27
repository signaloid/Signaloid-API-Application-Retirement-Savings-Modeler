# Create Retirement Savings Modeler application using Signaloid CLI

This guide will help you use the Signaloid CLI to create the Retirement Savings Modeler web application, as seen on the [Signaloid website](https://signaloid.com/industries/digital-banking#demo).

## Getting started

To clone this repository and its submodules:

```bash
git clone --recursive git@github.com:signaloid/Signaloid-API-Application-Retirement-Savings-Modeler.git
```

If you forgot to clone with `--recursive` and end up with empty submodule directories, you can fix this with:

```bash
git submodule update --init
```

## Using Signaloid CLI

Signaloid CLI generates a web front end for an existing C/C++ application.

Before you start, create a [Signaloid Cloud Developer Platform account](https://get.signaloid.io) and have your Signaloid API Key ready. Then visit the [Signaloid CLI documentation](https://docs.signaloid.io/docs/api/signaloid-cli/installation/) to find instructions on how to install Signaloid CLI.

### Generating an application

To generate a web application like the Retirement Savings Modeler, you need to initialize the web-app generator by running the command:

```bash
signaloid-cli init web-app
```

Signaloid CLI will prompt you for necessary configurations, such as your GitHub repository containing the C application and other project inputs. Once you provide this information, Signaloid CLI configures your project, allowing you to get the app up and running.

### Valid command-line arguments

Using valid command-line arguments is crucial for passing values between the web front end and the application. Enter when prompted the following command-line arguments for the Retirement Savings Modeler. Global argument ``-j`` generates the output in JSON format, while other arguments are required for each input to properly calculate the output.

| Parameter | Type | Flag |
|-----------|------|------|
| Print output | Global argument | ``-j`` |
| Number of years to retirement | Input | ``-n`` |
| Compounded annual interest rate | Input | ``-c``   |
| Annual contribution | Input | ``-t`` |
| Tax rate on interest | Input | ``-r`` |
| Withdrawal rate | Input | ``-w`` |

### Running the application

When you have completed all the prompts, the Signaloid CLI will have finished generating the application. Navigate to your new project and run the application:

```bash
cd <path-to-your-application-folder>
npm start
```

You can now open your browser and view the web application you've just built!

https://github.com/user-attachments/assets/e32e7b1d-c92f-40de-99ef-dda925f436e5
