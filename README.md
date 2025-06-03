# ClawCloud Run Templates

This repository serves as the official template repository for **ClawCloud Run** - a cloud-native application deployment platform. The provided templates enable users to seamlessly deploy various applications on ClawCloud Run with one click. Explore more at [ClawCloud Run](https://run.claw.cloud/).

## Template Structure

The template structure is organized as per the following directory tree:

- **Application Template File** (YAML format): Defines the Kubernetes and application resources.
  
- **Application README File** (Markdown format): Introduces the application and lists key features. Please do not include external links in the README file.
  
- **Application Screenshots** (PNG format): Displays the primary interface of the application.

```
App Name
├── index.yml
├── README.md
├── Picture1.png
├── Picture2.png
├── Picture3.png
└── ...
```

## Template Creation Guideline
- **Guidance**: Please follow [template-guidance.md](./template-guidance.md) as a tutorial.

- **Application Template File**: Refer to the sample file [template-example.yaml](./template-example.yaml) to create your application template, and test your template in App Store -> My Apps -> Debugging.

- **Readme File and Screenshots**: Ensure the Readme file and screenshots prominently showcase your application's core functions and key features.

## Template Submission

If you would like to contribute your application template to ClawCloud Run official App Store, you can follow these steps:

- Fork this repository and clone it to your local environment;

- Create a new directory for your application template, and remember to not capitalize the first letter of your application name;

- Create the files mentioned in the Template Structure section above;

- Commit your changes and submit a pull request to the main branch of this repository;

- After your pull request is merged, your application template will be published on ClawCloud Run's official App Store;

- You can also add a ClawCloud Run deploy button to your GitHub README or application docs, enabling users to deploy your application with one click.

![](./Run-on-ClawCloud.svg)

## Contributors

[![](https://contrib.rocks/image?repo=ClawCloud/Run-Template)](https://github.com/ClawCloud/Run-Template/graphs/contributors)

For additional collaboration opportunities or customized partnership inquiries, please contact our support team at `support@run.claw.cloud`.
