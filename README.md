# Relic CLI

**Forged through Rune. Built upon PHP.**

How to cast: a small runite to learn how a cast is spoken, how spells shape it, and how one cast can call another. Your first step out of the void.

**[Explore Rune ↗](https://github.com/devneet-id/rune)**
**[Explore Reliquary ↗](https://github.com/devneet-id/reliquary)**

---

## The Relic

This repo is a **relic**: a runite sealed as a `.rune`, listed in the **[Reliquary](https://github.com/devneet-id/reliquary)**.

| Relic | `.rune` | Carries |
| ----- | ------- | ------- |
| `devneet-id/relic-cli/cast` | `cast.rune` | the runite `cast` |

### Get it

**From the void** — a new folder, Rune and one awakening file:

```bash
composer require devneet/rune
```

```php
#!/usr/bin/env php
<?php
require_once __DIR__ . '/vendor/autoload.php';

Rune\Ethereal::awakening();
```

Save it as `cast`, then:

```bash
php cast
```

Answer `y`, and choose `devneet-id/relic-cli/cast`.

**Into a runite you already have:**

```bash
php cast reliquary --relic-runite=devneet-id/relic-cli/cast
```

**Or clone this repo:**

```bash
git clone https://github.com/devneet-id/relic-cli.git
cd relic-cli
composer install
php cast
```

---

## Made with Rune

This app is a **runite**: one file named `cast`, engraved from the origin runes of **[Rune](https://github.com/devneet-id/rune)**, a lore-driven, modular concept beneath PHP.

It uses only four runes:

| Rune | Role in this app |
| ---- | ---------------- |
| Aether | opens and closes the flow |
| Chanter | registers the casts and reads the spells |
| Weaver | fills the `{{tokens}}` of every message |
| Whisper | speaks to the user and asks for input |

Want to engrave your own? Start from the **[Rune repository](https://github.com/devneet-id/rune)**.

### Requirements

* PHP 8.1+
* Composer
* Rune 1.20+ *(for the reliquary)*

---

## Registered Casts

| Cast | Description |
| ---- | ----------- |
| `fire` | Shoot a fire ball. |
| `ice` | Shoot a blizzard. |
| `wind` | Shoot a wind blast. |
| `enchant --art --amount` | Cast one art many times. |
| `respell --total` | Cast random arts. |
| `with-name` | Ask a name, then cast for it. |

### Spells

| Spell | Cast | Value | Default |
| ----- | ---- | ----- | ------- |
| `--art` | `enchant` | `fire`, `ice` or `wind` | — (required) |
| `--amount` | `enchant` | how many times | `1` |
| `--total` | `respell` | how many random arts | `5` |

### Try it

```bash
php cast fire
php cast ice
php cast wind

php cast enchant
php cast enchant --art=fire
php cast enchant --art=ice --amount=3
php cast enchant --art=wind --amount=5
php cast enchant --art=thunder

php cast respell
php cast respell --total=10

php cast with-name

php cast grimoire
php cast grimoire --rune=Chanter
php cast fire --zero-trust
php cast fir
```

Every runite also carries the built-in casts of Rune: `grimoire`, `reliquary` and `sentinel`.

---

## What you learn

| Cast | Lesson |
| ---- | ------ |
| `fire`, `ice`, `wind` | a cast and its echo |
| `enchant` | read spells first, then cast another cast from code |
| `respell` | set a spell from code, the next cast reads it |
| `with-name` | ask the user, then chain casts |

**Every cast is a door, open them one by one.**

---

## References

* [Rune](https://github.com/devneet-id/rune) — Application foundation and tooling.
* [Rune Lore](https://github.com/devneet-id/rune-lore) — The full documentation, from the void to the beyond.
* [Reliquary](https://github.com/devneet-id/reliquary) — The relics of Rune.

---

**Built to create. Designed to evolve.**

**DEVNEET ©**
