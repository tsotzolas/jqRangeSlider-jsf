# jqRangeSlider-jsf
Jsf component for JqRangeSlider

JSF 2.2 component for the JqRangeSlider jQuery plugin (https://ghusse.github.io/jQRangeSlider/) for dates

The current version is 1.0 and is bundled with Timeago 1.5.4.
Usage


In your XHTML files add the following namespace:

xmlns:ta="http://tsotzolas.com/tags"

Now you can use the component by passing a java.util.Date using the value attribute:

                <ta:jqslider
                        mindate="#{bean.minDate}"
                        maxdate="#{bean.maxDate}"
                        mindefaultdate="#{bean.minDefaultDate}"
                        maxdefaultdate="#{bean.maxDefaultDate}"
                        for="slider"/>
                <h:inputHidden id="slider" value="#{bean.sliderValue}" />
                
                
                
                

jQuery / JSF component library integration

The component will take care of loading jQuery. It tries to integrate with JSF component libraries that also rely on jQuery, so you won't end up with multiple / conflicting jQuery versions.

Supported JSF component libraries at this moment:

    PrimeFaces

If you are not using one of these libraries, it will load the bundled version of jQuery.
