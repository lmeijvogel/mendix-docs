---
title: "Modules"
url: /refguide7/modules/
category: "Desktop Modeler"
#If moving or renaming this doc file, implement a temporary redirect and let the respective team know they should update the URL in the product. See Mapping to Products for more details.
---

## 1 Introduction

A Mendix project consists of modules: a **System** module, a [UI resources package](/refguide7/ui-resources-package/), and one or more user-defined modules. Modules are a way to split the functionality of your application into separate parts. For example, a web shop can put order management in a different module than customer and product management. The Modeler does not enforce any kind of module structure; it is up to you to choose logical modules for your application.

A module always contains exactly one [domain model](/refguide7/domain-model/). The domain model is a data model that describes the information in your application domain in an abstract way.

Within a module you can define [module security](/refguide7/module-security/) via module roles and specify security settings of those module roles for pages, microflows, entities and datasets.

Furthermore, a module can contain many different types of documents. Each type of document is described in its own domain-specific language (DSL). For example, user-interface forms are described by using a visual language with elements like text boxes, tables and grids. Below you see tables grouped by category of all the different kinds of documents you can create within a module.

## 2 Common

| Document type | Typical elements | Description |
| --- | --- | --- |
| [Pages](/refguide7/pages/) | [Data view](/refguide7/data-view/), [Data grid](/refguide7/data-grid/), [Table](/refguide7/table/), [Text box](/refguide7/text-box/) | Forms are used to create a user interface for the end user. They are composed of components that are called widgets. |
| [Microflows](/refguide7/microflows/) | [Activities](/refguide7/activities/), [Sequence Flow](/refguide7/sequence-flow/) | Microflows describe the logic of your application. They are composed of activities that manipulate objects, interact with the client etcetera. |
| [Enumerations](/refguide7/enumerations/) |   | An enumeration is a set of predefined values, for example: in a webshop, an enumeration called MemberType could have the values Gold and Silver. |

## 3 Page Resources

| Document type | Description |
| --- | --- |
| [Images](/refguide7/images/) | Images can be used to brighten up your application. Navigation items and the various kinds of buttons have small images (icons) to left of their captions. |
| [Layouts](/refguide7/layout/) | Layouts specify what comes where. Each  [page](/refguide7/page/) is based on a layout. The layout contains widgets and structures that return on every page based on that layout.  |
| [Menus](/refguide7/menu/) | A menu document defines a navigation menu that can be used by a  [menu widget](/refguide7/menu-widgets/). |
| [Snippets](/refguide7/snippet/) | Snippets define reusable interface parts. They can be used on  [pages](/refguide7/page/) and  [layouts](/refguide7/layout/) . |

## 4 Resources

| Document type | Description |
| --- | --- |
| [Constants](/refguide7/constants/) | Constants are used to define a constant value, for example: to store an URL to a webservice. |
| [Datasets](/refguide7/data-sets/) | A dataset can be used for reporting and is defined using either an OQL query or a custom Java action. |
| [Document Templates](/refguide7/document-templates/) | Document Templates are used to model a template needed as input for a document export action which can generate all kinds of documents based on application data. They are composed much in the same way as Forms. |
| [Java Actions](/refguide7/java-actions/) | With Java actions you can extend the functionality of your application in situations where it would be hard to implement this functionality in microflows. You can call a Java action from a microflow. |
| [Regular Expressions](/refguide7/regular-expressions/) | A regular expression describes a set of criteria that a string can match. |
| [Rules](/refguide7/rules/) | A rule defines a set of criteria, with a certain input the rule will result in a boolean or enumeration depending on the criteria met. It can be called from an exclusive split to determine the direction the microflow should go once the exclusive split is reached. |
| [Scheduled Events](/refguide7/scheduled-events/) | A scheduled event is used to execute a microflow at a certain point in time. You can also schedule it to repeat after a given time. For example, a scheduled event can run every morning at 6 A.M. |

## 5 Consumed Services

| Document type | Description |
| --- | --- |
| [Consumed Web Services](/refguide7/consumed-web-services/) | Importing web services of other applications (Mendix or otherwise) allows you to call those web services from your microflows. |
|  | A domain-to-XML mapping defines a translation from domain model objects to XML objects. |
|  | An XML-to-domain mapping defines a translation from XML objects to domain model objects. |
| [XML Schemas](/refguide7/xml-schemas/) | An XML schema is defined in an XML Schema Definition (XSD) file and can be imported in your model. It describes what a certain XML document should look like. |

## 6 Published Services

| Document type | Description |
| --- | --- |
| [Published OData Services](/refguide7/published-odata-services/) | Persistable entities can be exposed as an OData resource, so that they can be imported by third-party applications such as Excel. |
| [Published Web Services](/refguide7/published-web-services/) | A microflow can be published as a web service operation so that it can be called by third-party applications. |
