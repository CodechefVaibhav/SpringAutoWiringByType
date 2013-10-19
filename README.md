SpringAutoWiringByType
======================

Auto-wiring in Spring byType

Spring container looks at the beans on which autowire attribute is set to byType in the XML 
configuration file. It then tries to match and wire a property if its type matches with exactly 
one of the beans name in configuration file. If matches are found, it will inject those beans 
otherwise, it will throw exceptions.

As in our example , it hardly matters even if the variable is defined in TextEditor Class. for e.g
texteditor class doesn't contain any variable of type MyClass then also its constructor is called
even though it is not linked with this class through any means.

All the beans classes are instantiated which are defined applicationContext.xml file.

Try even commenting out everything related to SpellChecker class defined in class TextEditor class
& then run code then also SpellChecker will be instantiated.
