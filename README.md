# Punch-Out!! Champion Edition

Play as any boxer from *Mike Tyson's Punch-Out!!*, against the computer or a friend. Champion Edition replaces the campaign with a fighter-select menu and individual matches. Pick a boxer, fight, then head back to the menu for another matchup.

One side is always Little Mac, but either player can control him. If you're playing alone as an opponent, Mac has his own AI to fight back.

[Download v0.1](https://raw.githubusercontent.com/jtx/PunchOutChampionEdition/master/punchout-champion-edition-v0.1.ips) · [Installation](https://github.com/jtx/PunchOutChampionEdition#installation) · [Game modes](https://github.com/jtx/PunchOutChampionEdition#game-modes) · [Controls](https://github.com/jtx/PunchOutChampionEdition#controls) · [Move lists](https://github.com/jtx/PunchOutChampionEdition#move-lists)

This download contains an IPS patch. You'll need your own copy of the original ROM to use it.

## Screenshots

| Title screen | Single Player |
| :---: | :---: |
| ![Champion Edition title screen](https://raw.githubusercontent.com/jtx/PunchOutChampionEdition/master/assets/screenshots/title.png) | ![Single-player selection with Soda Popinski](https://raw.githubusercontent.com/jtx/PunchOutChampionEdition/master/assets/screenshots/single-player.png) |
| **Two-player character select** | **Tyson versus Mac** |
| ![Player 1 choosing Tyson and Player 2 choosing Mac](https://raw.githubusercontent.com/jtx/PunchOutChampionEdition/master/assets/screenshots/character-select.png) | ![Player 1 as Tyson fighting Player 2 as Mac](https://raw.githubusercontent.com/jtx/PunchOutChampionEdition/master/assets/screenshots/two-player-fight.png) |

## The roster

Little Mac, Glass Joe, Von Kaiser, Piston Honda, Don Flamenco, King Hippo, Great Tiger, Bald Bull, Soda Popinski, Mr. Sandman, Super Macho Man and Mike Tyson are all playable.

Honda, Don and Bull use their tougher rematch versions. There aren't separate roster slots for their first and second fights.

The opponents keep their signature moves: Bull Charge, Tiger's magic punches, Sandman's triple uppercut, Macho Man's spins and the rest. Some punches and evasions have mirrored versions so you can use them on either side. Their damage, weaknesses and knockdown rules still come from the original game.

The new menus use portraits from the game, with player markers and a glove-punch transition into the fight. The original intro and music are still here, and Tyson has an updated bald head and face tattoo.

## Installation

### Required original ROM

| Property | Required value |
| --- | --- |
| Game / revision | Mike Tyson's Punch-Out!! (Japan, USA) (Rev A) |
| Common alternate filename | `Mike Tyson's Punch-Out!! (U) (PRG1) [!].nes` |
| File format | iNES, including its 16-byte header, with no trainer |
| Full file size | 262,160 bytes |
| Full-file CRC32 | `3DF8E170` |
| Full-file SHA-1 | `0F0C2C2E294FF8CE255A618964728C935FD8963B` |

Check the checksum rather than relying on the filename. PRG0, the European release and the Mr. Dream version won't work with this patch.

### Apply the patch

1. Download the IPS and make a copy of your matching original ROM.
2. Open [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/) or another IPS patcher. Select the original `.nes` and `punchout-champion-edition-v0.1.ips`.
3. Apply the patch and save it as a new `.nes` file. Leave the 16-byte header intact. Always patch a clean original, not a previous Champion Edition build.
4. Load the patched `.nes` in your emulator. For RetroArch, use a NES core with MMC2 support, such as Nestopia UE. Set up both controller ports for Two Players.

The finished file should be 262,160 bytes with CRC32 `63444EAE`. [Full checksums are below](https://github.com/jtx/PunchOutChampionEdition#checksums). IPS won't catch a wrong source ROM for you, so check these if the game doesn't boot correctly.

Start fresh after patching rather than loading a save state from another version.

## Game modes

### Single Player

Choose Little Mac and the game picks a random opponent with his original AI. Choose anyone else and you'll fight CPU Mac.

After the match, you can return to character select and pick again. There's no campaign or password progression.

### Two Players

Both players choose a fighter. Since one side has to be Mac, the game sorts out conflicting choices:

| Selections | Final matchup |
| --- | --- |
| One Mac, one opponent | Both players keep their choices. |
| Both choose Mac | One player randomly keeps Mac; the other receives a random opponent. |
| Both choose opponents | One player randomly becomes Mac; the other keeps their chosen opponent. |

Either controller can be Mac. Boss-versus-boss fights aren't supported, and v0.1 doesn't keep a win tally.

## Controls

These are NES button names. Bind **B to your left punch button and A to your right punch button** in your emulator; keyboard bindings depend on your setup.

### Menus

| Screen | Input | Action |
| --- | --- | --- |
| Introduction | Start | Skip to the title |
| Title | Up / Down, then A | Choose and confirm Single Player or Two Players |
| Character select | D-pad | Move your selection |
| Character select | A | Ready your fighter |
| Character select | B | Cancel readiness |
| Character select | Select | Return to the title before everyone is ready; P1 in Single Player, either pad in Two Players |
| Pre-fight portraits | Start on Mac's controller | Begin the fight; use P1 Start when Mac is CPU-controlled |
| Match result | P1 A / P1 B | Return to character select / title |

Once everyone is ready, the glove animation plays and the game moves to the pre-fight screen.

### Little Mac

Mac uses his original controls. Hold Up for head punches.

| Input | Action |
| --- | --- |
| B | Left body punch |
| A | Right body punch |
| Up + B | Left head punch |
| Up + A | Right head punch |
| Left / Right | Dodge left / right |
| Down | Block |
| Start | Star uppercut; requires a star |
| Select between rounds | Extra recovery from Doc, once per bout |

Use your emulator's pause button; Start throws a star punch.

### Shared opponent controls

For the other boxers, B punches from the left side of the screen and A punches from the right. Since they face the camera, that's the reverse of their own left and right hands.

| Input | Action |
| --- | --- |
| B | Screen-left basic punch |
| A | Screen-right basic punch |
| Down + B | Screen-left secondary punch |
| Down + A | Screen-right secondary punch |
| Hold Up, without a punch | High guard |
| Hold Down, without a punch | Low guard |
| Left / Right | Evasion, where available; see each boxer below |
| Select, Up + Select, Down + Select | Specials and taunts; see move lists |

Release and press again for each move. You can't start another attack while being hit or recovering, and holding a button won't repeat it. Multi-punch specials have to finish before you can do something else.

## Move lists

Every opponent uses Up/Down to guard. In the lists below, B / A means screen-left / screen-right; adding Down keeps the same side.

<details>
<summary>Glass Joe</summary>

| Input | Move |
| --- | --- |
| B / A | Straight punches |
| Down + B / Down + A | Hooks |
| Left / Right | Left / right dodge |
| Select | Taunt |

</details>

<details>
<summary>Von Kaiser</summary>

| Input | Move |
| --- | --- |
| B / A | Jabs |
| Down + B / Down + A | Uppercuts |
| Right | Original duck/lean |
| Left | Mirrored duck/lean |
| Select | Unassigned |

Kaiser's evasion is a duck/lean rather than a full sidestep. Select has no special move.

</details>

<details>
<summary>Piston Honda</summary>

| Input | Move |
| --- | --- |
| B / A | Basic punches |
| Down + B | Original screen-left uppercut |
| Down + A | Mirrored screen-right uppercut |
| Right / Left | Original lean / mirrored lean |
| Select | Bow, then four fast punches and two uppercuts |
| Down + Select | Feinting uppercut |

</details>

<details>
<summary>Don Flamenco</summary>

| Input | Move |
| --- | --- |
| B / A | Straights |
| Down + B / Down + A | Hooks |
| Right / Left | Original evasion / mirrored evasion |
| Select | Stronger uppercut |
| Down + Select | Taunt/pose |
| Up + Select | Unassigned |

</details>

<details>
<summary>King Hippo</summary>

| Input | Move |
| --- | --- |
| B / A | Basic punches |
| Down + B / Down + A | Heavy punches |
| Select | Taunt |
| Down + Select | Side-to-side shuffle |
| Left / Right | Unassigned; no dodge |
| Up + Select | Unassigned |

The shuffle doesn't dodge attacks. Hippo still has his mouth/belly weakness and goes down for good after one knockdown.

</details>

<details>
<summary>Great Tiger</summary>

| Input | Move |
| --- | --- |
| B / A | Jabs |
| Down + B / Down + A | Uppercuts |
| Right / Left | Original lean / mirrored lean |
| Select | Magic attack sequence |
| Down + Select | Alternate uppercut stance |
| Up + Select | Unassigned |

The alternate uppercut stance has the same strength and speed. The magic sequence can keep going until it's blocked or someone is knocked down.

</details>

<details>
<summary>Bald Bull</summary>

| Input | Move |
| --- | --- |
| B / A | Jabs |
| Down + B / Down + A | Uppercuts |
| Right / Left | Original duck/lean / mirrored duck/lean |
| Select | Bull Charge |
| Up + Select | Heavy punch |
| Down + Select | Short bob/taunt |

The Bull Charge can still be countered with a well-timed body punch.

</details>

<details>
<summary>Soda Popinski</summary>

| Input | Move |
| --- | --- |
| B / A | Hooks |
| Down + B / Down + A | Uppercuts |
| Right / Left | Original evasion / mirrored evasion |
| Select | Repeating punch |
| Down + Select | Feint/taunt |
| Up + Select | Unassigned |

Hits or blocks can end the repeating punch early. The feint doesn't deal damage.

</details>

<details>
<summary>Mr. Sandman</summary>

| Input | Move |
| --- | --- |
| B / A | Regular punches |
| Down + B / Down + A | Uppercuts |
| Left / Right | Evasions, which can lead into counterpunches |
| Select | Triple uppercut sequence |
| Up + Select | Screen-right heavy uppercut |
| Down + Select | Screen-left heavy uppercut |

Sandman's Select super no longer waits through the AI's random delay before starting. It still has its normal windup and recovery.

</details>

<details>
<summary>Super Macho Man</summary>

| Input | Move |
| --- | --- |
| B / A | Basic punches |
| Down + B / Down + A | Uppercuts |
| Right / Left | Original evasion / mirrored evasion |
| Select | Single spin |
| Up + Select | Repeating super-spin sequence |
| Down + Select | Stepping feint into an uppercut |

You can't cancel a spin sequence into another move.

</details>

<details>
<summary>Mike Tyson</summary>

| Input | Move |
| --- | --- |
| B / A | Basic jabs |
| Down + B / Down + A | Uppercuts |
| Right / Left | Original evasion / mirrored evasion |
| Select | Alternate jab |
| Up + Select | Quick jab |
| Down + Select | Six-bob/flashing taunt |

Use Up/Down to block; Tyson won't guard for you. His opening-round knockout uppercuts are still just as dangerous. Only one quick-jab variant is assigned to a button.

</details>

## Compatibility and known issues

Tested with Nestopia and FCEUX, including browser play using the Nestopia core. For RetroArch, use a core that supports MMC2 (mapper 9).

The ROM keeps the original cartridge size and mapper. It hasn't been tested on a physical NES or flash cartridge yet. NTSC is the target; PAL hasn't been tested either. Online play would need your emulator's netplay support, which hasn't been tested with this release.

Balance is still being worked on. Some repeated-attack patterns can beat CPU Mac too easily, and Joe, Kaiser and Hippo need more testing against him. The boxers keep their original damage and weaknesses, so don't expect every matchup to be equally difficult.

Loading save states can cause audio issues, particularly across versions. If something behaves oddly after loading a state, try a fresh boot.

## Technical details

| Property | Value |
| --- | --- |
| Base game | Mike Tyson's Punch-Out!!, Rev A / PRG1 |
| Platform / language | NES / Famicom · English |
| Version | 0.1 |
| Patch format | IPS, applied directly to the clean headered original |
| ROM format | iNES 1.0, no trainer |
| Mapper | 9 — Nintendo MMC2 |
| PRG-ROM | 128 KiB |
| CHR-ROM | 128 KiB |
| Total file size | 262,160 bytes, including the 16-byte header |
| Expansion | No added ROM banks or RAM; original cartridge capacity retained |
| Input | Standard NES controller ports 1 and 2 |

### Checksums

<details>
<summary>Original ROM, patch and patched ROM</summary>

Clean original, including the iNES header:

```text
Size:    262160 bytes
CRC32:   3DF8E170
MD5:     C119A5A9B0E2959AD5D11562F9F4CE55
SHA-1:   0F0C2C2E294FF8CE255A618964728C935FD8963B
SHA-256: 60EF51F55F6ADDB7A1893F816AAD75EE3E146DD646958A865D3BECE5B429B600
```

If your database lists hashes without the header, the original payload is 262,144 bytes with CRC32 `2C818014` and SHA-1 `B6F6BD9D78CDD264A117D4B647AEE3309993E9A9`. Don't remove the header when patching.

IPS patch:

```text
File:    punchout-champion-edition-v0.1.ips
Size:    22647 bytes
CRC32:   B46CD879
SHA-1:   253C6FD6600A1817A7AA4D8897F1023A80A22E64
SHA-256: 4D02C0852E40A2D160B8EEA11A9ECCE7D671A1B499113E49DC3AF9609C93789B
```

Patched ROM, including the iNES header:

```text
Size:    262160 bytes
CRC32:   63444EAE
MD5:     7E194E04114C103C17D9C5DAA558BCA9
SHA-1:   1F1A8A65854D1EF0F52A5463261F75E443A04C8F
SHA-256: 42829245EF86A63BD28E08D5ECDAA7950FC1944A9D9B9868E6CD1D9D00F755AE
```

The patch has been checked against the original ROM and produces the file identified above.

</details>

## Feedback

Found a bug? Include your emulator and version, which boxer you were playing, the game mode, and how to reproduce it. Mention if you loaded a save state. Clips and screenshots help; please don't attach ROM files.

## License

Original game by Nintendo, 1987. Champion Edition is an unofficial fan project, not affiliated with Nintendo or Mike Tyson. No game ROM is included.

The [MIT license](https://github.com/jtx/PunchOutChampionEdition/blob/master/LICENSE) covers this project's original contributions, not Nintendo's game code, artwork or music.
