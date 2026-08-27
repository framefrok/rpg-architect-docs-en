# Enter Vehicle

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/102-enter-vehicle/*

---

# Enter Vehicle

## **Enter Vehicle**[¶](#enter-vehicle "Permanent link")

Boards the party onto a vehicle by its unique ID, optionally returning the party to the vehicle's saved location first.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Reboard Current Vehicle

Reboards the vehicle the party is currently inside. When enabled, the target vehicle and return option are ignored; does nothing if the party is not inside a vehicle.

Toggle

Return to Vehicle

Whether to teleport the party to the vehicle's saved location before boarding. When disabled, the vehicle must already be on the current map.

Toggle

Run Scripts

Whether to run the vehicle's before and after enter scripts.

Toggle

Vehicle

The unique ID of the vehicle to board.

[Variable or Value](../../../05-reference/variable-or-value/)