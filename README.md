# Global custom language keys

In a multi-lingual environment you often need to create your own labels/keys that are translated for multiple languages.  
This is often done in a specific module like a portlet.
Sometimes you want to share the language keys across multiple modules which is explained here (https://help.liferay.com/hc/en-us/articles/360029005932-Shared-Language-Keys)  

  
However, there's also an option to create them in a more global way.
Have a look at the code.  
For each language you need a ResourceBundle extension and a Language_xx_XX.properties file with the translated keys.
Nice thing is you can directly use the translated keys in your freemarker templates like `<@liferay.language key="custom.arrange.immediately" />`

Haven't tested it but it's likely you can also override existing keys so handle with care ;-)