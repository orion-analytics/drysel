# DrySel
“Automate the (Test) Automation” - with the help of "DrySel". 

## UI Test Automation - A view from 10000 Feet over the surface

```gherkin
given ANY user interface (UI)
when test data are provided
then the test should be executed
```

I believe test automation should be as simple as described in the story above. In the same light, I envision "DrySel" (or any other test automation framework/tool) as an __abstract machine__, which takes test objects (objects which describe UI and Test Data) as inputs and produces test results. What happens inside the machine or how the machine achieves the automation should remain opaque to its user. 

## So what is DrySel?

* __DrySel__ is a family of test automation frameworks and tools, developed based on a very basic software engineering principle of DRY - “Don’t Repeat Yourself”.

* From the bottom to top __DrySel__ is comprised of ...
1. [DrySelCore](https://github.com/orion-analytics/dryselcore) - the core framework, which realizes abstraction of the test automation and encapsulates “Selenium”. Now, you don’t need to write any Selenium-code! [DrySelCore.Demo](https://github.com/orion-analytics/dryselcore.demo) provides an example of how to user "DrySelCore".
2. [DrySelJSON](https://github.com/orion-analytics/dryseljson) - a framework, built on top of the “Core”. It pushes out definitions of Test Objects (UI and Data) from the programming boundaries of the “Core”, making it possible for programmers as well as non-programmers to contribute in defining “Test Objects” in easy to understand “JSON” objects. [DrySelJSON.Demo](https://github.com/orion-analytics/dryseljson.demo) provides an example of how to user "DrySelJson".
3. [DrySelMagic](https://github.com/orion-analytics/dryselmagic) - the ultimate tool for UI Automation. It removes the need to write “boiler-plate” code from both of above frameworks. Now, anyone can automate UI-Testing without writing a single line of programming code. [DrySelMagic.Demo](https://github.com/orion-analytics/dryselmagic.demo) provides an example of how to user "DrySelMagic".
