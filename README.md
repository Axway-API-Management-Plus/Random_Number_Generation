# Javascript-RNG
Sample Javascript Random Number Generator

## Description

This policy is meant to serve as a template for customers looking to enable some level of random number generation. This could be used as a framework to create pseudo-random pins for a second factor of mobile authentication for example, or perhaps to create a basic captcha or nonce type service.

The basic policy flow is as follows:

- **Scripting Language Filter**: This filter, renamed "Random Number Generation", uses JavaScript to generate a random one digit output. Additional comments about how this operates are built into the code to explain each piece of the operation. This output could be looped and concatenated to create multi-digit outputs.
- **Set Message Filter**: This filter, renamed "Return Random Number", take the output of the scripting filter and sets it in a message to return to the requestor.
- **Reflect Message Filter**: This filter returns the set message from above to the requestor.


## API Management Version ## API Management Version Compatibility
This artefact was successfully tested for the following versions:
- V7.5.3


## Install

```
• Download the randomNumberGenerator*.xml policy file.
• There are several options to import this file, including Team Development, REST API, and sample scripted options included with the Axway solution. The simplest way however is to open Policy Studio and select 'File --> Import --> Import Configuration Fragment'.
```

Import Dialog:

![alt text](https://github.com/Axway-API-Management-Plus/Random_Number_Generation/blob/master/example/src/importFrag.png "Import Fragment")

## Usage

```
• Import the RNG policy file.
• Set up an endpoint to call the policy.
• Execute the call through a testing tool to view the result.
```

Sample output:

![alt text](https://github.com/Axway-API-Management-Plus/Random_Number_Generation/blob/master/example/src/sampleOutput.png "Sample Output")

## Bug and Caveats

```
N/A
```

## Contributing

Please read [Contributing.md](https://github.com/Axway-API-Management/Common/blob/master/Contributing.md) for details on our code of conduct, and the process for submitting pull requests to us.


## Team

![alt text][Axwaylogo] Axway Team

[Axwaylogo]: https://github.com/Axway-API-Management/Common/blob/master/img/AxwayLogoSmall.png  "Axway logo"


## License
[Apache License 2.0](/LICENSE)
