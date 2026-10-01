# AtomicFuel API

Пакет событий: `com.atomicfuel.api`.

## AtomicFuelTickEvent

Вызывается каждый тик для активного реактора.

`getReactor()` возвращает `ReactorState`.

## AtomicFuelInstabilityEvent

Cancellable. Вызывается непосредственно перед запуском meltdown countdown.

## AtomicMeltdownStartEvent

Вызывается при начале 10-секундного countdown.

## AtomicExplosionEvent

Cancellable. Вызывается перед фактическим Minecraft explosion.

Если другое plugin-системное правило запрещает взрыв, можно `setCancelled(true)`.

## AtomicStabilizeEvent

Вызывается после успешной стабилизации реактора.

## RadiationZoneCreateEvent

Вызывается после создания RadiationZone.

## RadiationZoneExpireEvent

Вызывается при автоматическом истечении RadiationZone.

## PDC

Для интеграции ориентируйтесь на `NamespacedKey` AtomicFuel:

- `item` — тип кастомного предмета;
- `enrichment` — обогащение AtomicFuelRod;
- `energy` — заряд AtomicBattery;
- chunk PDC — метки кастомных блоков и энергетических буферов;
- world PDC — индексы реакторов и RadiationZone.
