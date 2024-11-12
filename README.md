# Basic MUnits for ACB

> [!IMPORTANT]
> **UPDATE (Oct '24 release)**
> 
> Make sure you're using any of the following Mule Runtime versions 
> - `4.6.7+`
> - `4.7.3+`
> - `4.8.0+`


Use this project to try out the MUnit visual functionality of ACB. There are 5 tests in total, one that fails on purpose.

Releases:
- **June '24 release**: test and debug existing MUnits.
- **October '24 release**: see the MUnit coverage visually.

Videos:
- [Support for Existing MUnit Tests in Anypoint Code Builder (June'24)](https://youtu.be/6Kvg4vNoR7s)

## Similar repos

[![](https://github-readme-stats.vercel.app/api/pin/?username=alexandramartinez&repo=my-process-api-munits&theme=holi)](https://github.com/alexandramartinez/my-process-api-munits)

## Enterprise credentials

**Updated after October '24 release:**

Make sure you're using Mule Runtime versions `4.6.7+`, `4.7.3+`, or `4.8.0+` to run MUnits without enterprise credentials.

<details>
<summary><i>Deprecated info (June '24 release)</i></summary>

*This information no longer applies but is kept here for the records.*

*~~Please note that you will need Enterprise credentials to access this feature on ACB.~~*

*~~To make sure your credentials work properly, go to [this link](https://repository.mulesoft.org/nexus/content/repositories/releases-ee/) and use your credentials to sign in.~~*

*~~You will use those credentials in your Maven's `settings.xml` file. You can use this [`example-settings.xml`](/example-settings.xml) file as a guide to set up your own or refer to [this link](https://help.salesforce.com/s/articleView?id=001114523&type=1) for more information.~~*

</details>

## MULE_EE for debugging

**Updated after October '24 release:**

Make sure you're using Mule Runtime versions `4.6.7+`, `4.7.3+`, or `4.8.0+` to run MUnits without enterprise credentials.

<details>
<summary><i>Deprecated info (June '24 release)</i></summary>

*This information no longer applies but is kept here for the records.*

*~~If you're running the `MULE_CE` (community edition) runtime, you will be able to run the tests but you won't be able to debug them.~~*

*~~To make sure you're running the enterprise edition, you can add the following line in your `mule-artifact.json`.~~*

```
"requiredProduct": "MULE_EE"
```

*~~Refer to [this file](/mule-artifact.json) for an example of how this looks like.~~*
</details>



## Other considerations

If you're running Mule 4.7+ and/or Java 17 for your project, make sure to use the latest versions of the **Mule Maven Plugin** and **MUnit**.

You can set these versions in your `pom.xml` and check the latest versions using the following links:
- [Mule Maven Plugin Release Notes](https://docs.mulesoft.com/release-notes/mule-maven-plugin/mule-maven-plugin-release-notes)
- [MUnit Release Notes](https://docs.mulesoft.com/munit/latest/munit-release-notes)
