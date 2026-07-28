# Scrap Mechanic Scrapyard Quest Bug Fix

This repository contains a temporary fix for the scrapyard quest bug.

It includes both a preventative fix for saves that have not encountered the bug and a custom console command to unlock the quest if the bug has already occurred.

## Apply the fix

1. Make sure the game is fully closed and is not running.
2. Open Steam.
3. Right-click the game, then select **Properties > General**.
4. Under **Launch Options**, enter `-dev` so the game can load modified files.

> [!CAUTION]
> Using `-dev` mode disables achievements. Remove the launch option to re-enable them.

5. Close the **Properties** window.
6. Right-click the game, then select **Manage > Browse local files**.

---

You should now be in your Scrap Mechanic installation folder.

Place the modified files in the following locations:

```text
Scrap Mechanic\Survival\Scripts\game\SurvivalGame.lua
Scrap Mechanic\Survival\Scripts\game\quests\ScrapyardQuest.lua
```

Once the files are in place, restart the game.

If everything worked correctly, developer mode should be enabled. You can verify this by entering `/help` in the in-game chat. It should display several *creative mode* commands.

You should also see a command named `/quest_bug_unlock`. This is the new command used to fix the bugged quest.

> [!CAUTION]
> Only use this command if the bug has already occurred. It forces the game to complete the bugged quest and activate the next one.
>
> This command has not been tested in any other scenario. I am not responsible for any damage it may cause to your save file.

---

## Remove the fix

To remove this fix and return to the regular version of Scrap Mechanic, use Steam’s **Verify integrity of game files** option. Steam should restore the original files.

If it does not, manually delete the modified files beforehand, then verify the game files again.
