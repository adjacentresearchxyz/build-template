# Build Template
An automated build template for various applications. This is an ever growing and changing template that is also flexible (use all the workflows or pick and choose!)

- SAST and DAST scans via [Fossa](https://fossa.com) and [StackHawk](https://stackhack.com)
- Docker build, sign, and publish to container registry

## Setup 
### Secrets 
Include the following secrets in your repository/account/organization with values being the api keys for the SAST and DAST platforms
- `HAWK_API_KEY`
- `fossaApiKey`

### Using Stackhack
[StackHawk](https://stackhack.com) performs scans and tests on running applications. Create a new application in the [StackHawk](https://stackhack.com) platform and include the `application-id` and the port of the application in the `stackhawk.yml` file to perform scans.

Note: There could very easily be applications in which [StackHawk](https://stackhack.com) is not a fit or something you need to consider. In that case you can disable the workflow (but make sure you still run some tests!)