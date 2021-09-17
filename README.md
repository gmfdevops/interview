# GMF Interview Assessment
You must **not** share this assessment directly on public forums for help.  However you are free to use any resources available on the internet to complete the tasks.

Pick one of the below assessments, perform it to completion, and after completion email it to the addresses provided by your recruiter.

Each of these assessments correlates to a different job role.  Do the one that you have the most interest in.  Feel free to do multiple if you like.

## Assessment 1: Brain teaser and docker skills assessment
### Coding the brain teaser
1. This can be done in any coding or scripting language of your choice.  PowerShell, C#, Python, JavaScript, etc...
    - You will also need to configure this to run in docker later.  Pick accordingly.
1. Your application will support input of any **odd** number >= 5
1. Your application will take the input and create an hourglass outlined in uppercase Xs.  You must use underscores as filler characters to make viewing easier than using spaces.
    - Your hourglass shape will always be the same height and width as the input number
    - The top and bottom row will always be the number of X's from your input
    - The middle will always come to a single X

```
Examples:
Input = 5
XXXXX
_X_X_
__X__
_X_X_
XXXXX

Input = 7
XXXXXXX
_X___X_
__X_X__
___X___
__X_X__
_X___X_
XXXXXXX
```

### Test your results
1. Configure a test to run your code from Part 1 against the inputs 5, 7, 15, 21 and output the results to the console.  I may change this to test other numbers as needed.  It must work for any odd number >= 5.

### Docker
1. Create a docker image that will build and run your code against the test scenarios above.
   - You should utilize docker best practices to make the runtime image as clean as possible.

### Prepare for live interview
1. We will ask you questions about why you used certain code or methods so you must understand how your code works
1. We will ask you about your container image and your testing methods
1. We will likely ask you additional questions about what would come next if you were preparing to build this in a pipeline for a production deployment
1. We will ask you about experience you have with using pipelines for enterprise software deployment

## Assessment 2: Terraform skills assessment
### Basic Terraform usage
1. This can be done using any version of Terraform, no external providers are required.
2. Create a Terraform configuration with a resource(s) that prints out locally a map of make and models listed below.
```
# Make      Model
Chevrolet   Suburban
Cadillac    Escalade
GMC         Yukon
```
3. Your configuration should be able to accept more than the make and model key value pairs listed above.

### Convert the configuration to a module
1. Create a module based on the configuration above. The module should accept a map of make and models as input and should output the resources created.
