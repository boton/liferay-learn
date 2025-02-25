# Using Liferay Util Include

The include tag lets you include other JSP files in your portlet's JSP, theme, or web content. This can increase readability as well as provide separation of concerns for JSP files. 

The `page` attribute is required and specifies the path to the JSP or JSPF to include. The `servletContext` refers to the request context that the included JSP should use. Passing `<%= application %>` to this attribute lets the included JSP use the same `request` object as other objects that might be set in the prior JSP. 

Below is an example configuration for the `<liferay-util:include>` tag:

```jsp
<liferay-util:include 
  page="/relative/path/to/file.jsp" 
  servletContext="<%= application %>"
/>
```

Now you know how to use the `<liferay-util:include>` tag to include other JSPs in your portlets, themes, and web content. 

## Related Topics

* [Using the Liferay Util Param Tag](./liferay-util-param.md)
* [Using the Liferay Util Dynamic Include Tag](./liferay-util-dynamic-include.md)
* [Using the Liferay Front-End Taglibs](../clay-tag-library.md)