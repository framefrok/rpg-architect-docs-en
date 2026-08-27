# Set User Interface Element Context

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/101-set-user-interface-element-context/*

---

# Set User Interface Element Context

## **Set User Interface Element Context**[¶](#set-user-interface-element-context "Permanent link")

Sets or change the data context on a specific user interface element.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Child Context

The name of the child property to use as the context.

String

Context

The context provider to use for supplying data to the element.

[User Interface Context](../../../10-user-interfaces/user-interface-context/)

Context Filters

The filter groups to apply to the context.

[Filter](../../../05-reference/filter/)

Local

Whether the variable for the unique ID is local or global.

Toggle

Source

The data source to look up the context object from using a unique ID.

[Data Source](../../../08-data-sources/)

Use Child Context

Whether to use a child property of the current context as the new context.

Toggle

Use Context

Whether to use a context provider to supply data to the element.

Toggle

Use Current Selection Context

Whether to use the context of the current selection on the user interface element.

Toggle

Use Filters Only

Whether to apply filters to the existing context without changing the context itself.

Toggle

Use Unique ID and Source

Whether to look up the context from a data source using a unique ID stored in a variable.

Toggle

User Interface Element

The unique ID of the user interface element to set the context on.

[Variable or Value](../../../05-reference/variable-or-value/)

Variable Index

The index of the variable that contains the unique ID for the data source lookup.

Number

## **Examples**[¶](#examples "Permanent link")

#### **Set Element Context to the Current Selection**[¶](#set-element-context-to-the-current-selection "Permanent link")

This sets the context of the element whose unique ID is stored in Global Variable 0 to the current selection context.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_ui_element_context($gv[0], current);`

`[](#__codelineno-1-1){"Data":{"ChildContext":null,"ContextFilterGroups":[],"ContextProvider":null,"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IsLocal":0,"Source":null,"UseChildContext":0,"UseContext":0,"UseContextFiltersOnly":0,"UseCurrent":1,"UseDataSource":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.SetUserInterfaceElementContextCommand"}`

#### **Set Element Context Using a Child Property**[¶](#set-element-context-using-a-child-property "Permanent link")

This sets the context of the element to a child property named 'Inventory' from the current context.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_ui_element_context($gv[0], child("Inventory"));`

`[](#__codelineno-3-1){"Data":{"ChildContext":"Inventory","ContextFilterGroups":[],"ContextProvider":null,"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IsLocal":0,"Source":null,"UseChildContext":1,"UseContext":0,"UseContextFiltersOnly":0,"UseCurrent":0,"UseDataSource":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.SetUserInterfaceElementContextCommand"}`

#### **Set Element Context from a Data Source Using a Unique ID**[¶](#set-element-context-from-a-data-source-using-a-unique-id "Permanent link")

This sets the context of the element by looking up a hero from the data source using the unique ID stored in Global Variable 1.

Code ScriptVisual Script

`[](#__codelineno-4-1)set_ui_element_context($gv[0], data_source(hero, $gv[1]));`

`[](#__codelineno-5-1){"Data":{"ChildContext":null,"ContextFilterGroups":[],"ContextProvider":null,"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":1,"IsLocal":0,"Source":{"$":"HeroDataSource","ParameterIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"HeroProperty":0,"IsLocal":0,"SourceIndex":0,"Metadata":null},"UseChildContext":0,"UseContext":0,"UseContextFiltersOnly":0,"UseCurrent":0,"UseDataSource":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.SetUserInterfaceElementContextCommand"}`