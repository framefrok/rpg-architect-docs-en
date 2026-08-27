# Local and Global Data

*Источник: https://docs.rpg-architect.com/05-reference/local-and-global-data/*

---

# Local and Global Data

## **Local and Global Data**[¶](#local-and-global-data "Permanent link")

[Switches](../switch/) and [Variables](../variable/) exist in two scopes that determine their lifetime and visibility.

### Global[¶](#global "Permanent link")

Global switches and variables persist throughout the entire game instance, regardless of location or context. They are the default scope and are accessible from any script on any map. This is the traditional approach used by most RPG engines.

### Local[¶](#local "Permanent link")

Local switches and variables belong to individual [Entities](../entity/). Each entity instance maintains its own independent set of local data. When the entity is no longer active, its local data is removed — unless the entity is configured to persist its local data.

Local data is useful for prefabricated entities that share the same scripts but need independent state. For example, multiple enemies of the same type can each track their own "is alive" switch independently.

> **Note**: Use **Is Local Data Persisted** on an entity to keep its local switches and variables across map transitions.
> 
> **Note**: Use **Is All Data Persisted** to additionally persist position and other runtime state.