# Quality Factor (McCall’s factor model)

There is a need for a comprehensive definition of requirements that will cover all attributes of software and aspects of the use of software, including usability aspects, reusability aspects, maintainability aspects, and so forth in order to assure the full satisfaction of the users.

All example will be using social media app.

## Product operation factors

### Correctness

Software system’s required outputs.

Example: The message sent must be the same as the message received.

### Reliability

Deal with failures to provide service and determine the maximum allowed software system failure rate.

Example: The service uptime is 99% per year.

### Efficiency

Deal with the hardware resources needed or sometimes deals with the time between recharging of the system’s portable computer. The requirements may include the maximum values at which the hardware resources will be applied in the developed software system or the firmware.

### Integrity

Deal with the software system security. Requirements to prevent access to unauthorized person.

Example: Only the sender and recipient of the message can see the message.

### Usability

Deal with the scope of staff resources needed to train a new employee and to operate the software system.

## Product revision factors

### Maintainability

Determine the efforts that will be needed by users and maintenance personnel to identify the reasons for software failures, to correct the failures, and to verify the success of the corrections.

Example: A module should only take one responsibility.

### Flexibility

Efforts required to support adaptive maintenance activities are covered by the flexibility requirements.

Example: Onboarding should only take 5 minutes for new user.

### Testability

Testability requirements related to software operation include automatic diagnostics performed by the software system prior to starting the system, to find out whether all components of the software system are in working order and to obtain a report about the detected faults.

Example: Each deployment should pass the test.

## Product transition factors

### Portability

Adaptation of a software system to other environments consisting of different hardware, different operating systems, and so forth.

Example: The app should work across multiple platform.

### Reusability

Deal with the use of software modules originally designed for one project in a new software project currently being developed. The reuse of software is expected to save development resources, shorten the development period, and provide higher quality modules.

Example: The app should consist of smaller module.

### Interoperability

Specify the name(s) of the software or firmware for which interface is required. They can also specify the output structure accepted as standard in a specific industry or applications area.

Example: The app api endpoint should follow REST api standard route.

## Alternative models of software quality factors

- The Evans and Marciniak factor model (Evans and Marciniak, 1987).
- The Deutsch and Willis factor model (Deutsch and Willis, 1988).

## New Suggested Factors

### Verifiability

Most verifiability requirements refer to modularity, to simplicity, and to adherence to documentation and programming guidelines.

### Expandability

Refer to future efforts that will be needed to serve larger populations, improve service, or add new applications in order to improve usability. The majority of these requirements are covered by McCall’s flexibility factor.

### Safety

Are meant to eliminate conditions hazardous to operators of equipment as a result of errors in process control software.

### Manageability

Refer to the administrative tools that support software modification during the software development and maintenance periods, such as environment variables.

### Survivability

These define the minimum time allowed between failures of the system, and the maximum time permitted for recovery of service, two factors that pertain to service continuity. Similar with the reliability factor described in McCall’s model.
