# Basic MUnits for ACB

In the June '24 release of ACB, a new functionality to test existing MUnits was introduced. Use this project to try it out!

There are 5 tests in total, one that fails on purpose.

For more information, check out [this demo](https://youtu.be/6Kvg4vNoR7s).

## Enterprise credentials

Please note that you will need Enterprise credentials to access this feature on ACB. 

To make sure your credentials work properly, go to [this link](https://repository.mulesoft.org/nexus/content/repositories/releases-ee/) and use your credentials to sign in.

You will use those credentials in your Maven's `settings.xml` file. You can use this [`example-settings.xml`](/example-settings.xml) file as a guide to set up your own or refer to [this link](https://help.salesforce.com/s/articleView?id=001114523&type=1) for more information.

## MULE_EE for debugging

If you're running the `MULE_CE` (community edition) runtime, you will be able to run the tests but you won't be able to debug them.

To make sure you're running the enterprise edition, you can add the following line in your `mule-artifact.json`.

```
"requiredProduct": "MULE_EE"
```

Refer to [this file](/mule-artifact.json) for an example of how this looks like.

## Other considerations

If you're running Mule 4.7 and/or Java 17 for your project, make sure to use the latest versions of the **Mule Maven Plugin** and **MUnit**.

You can set these versions in your `pom.xml` and check the latest versions using the following links:
- [Mule Maven Plugin Release Notes](https://docs.mulesoft.com/release-notes/mule-maven-plugin/mule-maven-plugin-release-notes)
- [MUnit Release Notes](https://docs.mulesoft.com/munit/latest/munit-release-notes)