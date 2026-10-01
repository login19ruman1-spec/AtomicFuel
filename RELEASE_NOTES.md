# Команды AtomicFuel

## Администратор

### Выдать предмет

```text
/atomicfuel give <player> <type> [amount]
```

Пример:

```text
/atomicfuel give Steve atomic_fuel_rod 9
```

### Статус ближайшего реактора

```text
/atomicfuel status
```

Показывает:

- температуру;
- стабильность;
- обогащение;
- ControlRod;
- CoolantCell;
- NeutronReflector;
- состояние countdown.

### Стабилизация

```text
/atomicfuel stabilize
```

Действует на ближайший реактор в радиусе 64 блоков.

### Очистка радиации

```text
/atomicfuel cleanup <radius>
```

Пример:

```text
/atomicfuel cleanup 100
```

### Перезагрузка

```text
/atomicfuel reload
```

## Права

```text
atomicfuel.admin
atomicfuel.use
atomicfuel.craft
```

По умолчанию:

- `atomicfuel.admin` — OP;
- `atomicfuel.use` — true;
- `atomicfuel.craft` — true.
