# Comparing `tmp/pmdsky_debug_py-5.1.9-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-6.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 784105 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Apr-03 04:25 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Apr-03 04:25 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   720789 b- defN 23-Apr-03 04:25 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   688659 b- defN 23-Apr-03 04:25 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   709748 b- defN 23-Apr-03 04:25 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   688659 b- defN 23-Apr-03 04:25 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   727240 b- defN 23-Apr-03 04:25 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   688670 b- defN 23-Apr-03 04:25 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   229717 b- defN 23-Apr-03 04:25 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:25 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Apr-03 04:26 pmdsky_debug_py-5.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 04:26 pmdsky_debug_py-5.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-03 04:26 pmdsky_debug_py-5.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Apr-03 04:26 pmdsky_debug_py-5.1.9.dist-info/RECORD
-14 files, 4457926 bytes uncompressed, 782207 bytes compressed:  82.5%
+Zip file size: 846702 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jun-27 04:28 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-27 04:28 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   778781 b- defN 23-Jun-27 04:28 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   745826 b- defN 23-Jun-27 04:28 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   766901 b- defN 23-Jun-27 04:28 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   745826 b- defN 23-Jun-27 04:28 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   786248 b- defN 23-Jun-27 04:28 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   745837 b- defN 23-Jun-27 04:28 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   243251 b- defN 23-Jun-27 04:28 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 04:28 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jun-27 04:29 pmdsky_debug_py-6.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 04:29 pmdsky_debug_py-6.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-27 04:29 pmdsky_debug_py-6.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Jun-27 04:29 pmdsky_debug_py-6.0.0.dist-info/RECORD
+14 files, 4817114 bytes uncompressed, 844804 bytes compressed:  82.5%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-5.1.9.dist-info/METADATA
+Filename: pmdsky_debug_py-6.0.0.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-5.1.9.dist-info/WHEEL
+Filename: pmdsky_debug_py-6.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-5.1.9.dist-info/top_level.txt
+Filename: pmdsky_debug_py-6.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-5.1.9.dist-info/RECORD
+Filename: pmdsky_debug_py-6.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.5.1+f276906247"
+RELEASE = "v0.6.0+aa2e93eb51"
```

## pmdsky_debug_py/eu.py

```diff
@@ -1033,17 +1033,17 @@
 
     LoadFileInPackWithPackId = Symbol(
         [0xC3E4],
         [0x200C3E4],
         None,
         (
             "Call LoadFileInPack after looking up the global Pack archive by its"
-            " identifier\n\nr0: pack file identifier\nr1: [output] target buffer\nr2:"
-            " file index\nreturn: number of read bytes (identical to the length of the"
-            " pack from the Table of Content)"
+            " identifier\n\nr0: pack file identifier\nr1: file index\nr2: [output]"
+            " target buffer\nreturn: number of read bytes (identical to the length of"
+            " the pack from the Table of Content)"
         ),
     )
 
     AllocAndLoadFileInPack = Symbol(
         [0xC410],
         [0x200C410],
         None,
@@ -1084,14 +1084,27 @@
             "Load the indexed file from the Pack archive, itself loaded from the"
             " ROM.\n\nr0: pack file struct\nr1: [output] target buffer\nr2: file"
             " index\nreturn: number of read bytes (identical to the length of the pack"
             " from the Table of Content)"
         ),
     )
 
+    GetDungeonResultMsg = Symbol(
+        [0xC584],
+        [0x200C584],
+        None,
+        (
+            "Gets the message that is shown on the dungeon results ('The Last Outing')"
+            " screen, right after the leader's name.\n\nr0: Damage source value to use"
+            " when displaying the cause of fainting or the result of the"
+            " expedition\nr1: [output] Buffer where the resulting message will be"
+            " stored\nr2: Buffer size\nr3: (?) Seems to point to a buffer"
+        ),
+    )
+
     GetDamageSource = Symbol(
         [0xCADC],
         [0x200CADC],
         None,
         (
             "Gets the damage source for a given move-item combination.\n\nIf there's no"
             " item, the source is the move ID. If the item is an orb, return"
@@ -1169,14 +1182,26 @@
         None,
         (
             "Checks if an item is one of the aura bows received at the start of the"
             " game.\n\nr0: item ID\nreturn: bool"
         ),
     )
 
+    IsTreasureBox = Symbol(
+        [0xCD0C],
+        [0x200CD0C],
+        None,
+        (
+            "Checks if the given item ID is a treasure box\n\nIn particular, it checks"
+            " if the category of the item is CATEGORY_TREASURE_BOXES_1,"
+            " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
+            " ID\nreturn: True if the item is a treasure box, false otherwise"
+        ),
+    )
+
     InitItem = Symbol(
         [0xCF24],
         [0x200CF24],
         None,
         (
             "Initialize an item struct with the given information.\n\nThis will resolve"
             " the quantity based on the item type. For Poké, the quantity code will"
@@ -1496,22 +1521,21 @@
     GetItemMoveId = Symbol(
         [0xEB28],
         [0x200EB28],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: move ID",
     )
 
-    TestItemFlag0xE = Symbol(
+    TestItemAiFlag = Symbol(
         [0xEB48],
         [0x200EB48],
         None,
         (
-            "Tests bit 7 if r1 is 0, bit 6 if r1 is 1, bit 5 otherwise\n\nNote:"
-            " unverified, ported from Irdkwia's notes\n\nr0: item ID\nr1:"
-            " bit_id\nreturn: bool"
+            "Used to check the AI flags for an item. Tests bit 7 if r1 is 0, bit 6 if"
+            " r1 is 1, bit\n5 otherwise.\n\nr0: item ID\nr1: bit_id\nreturn: bool"
         ),
     )
 
     IsItemInTimeDarkness = Symbol(
         [0xEBD8],
         [0x200EBD8],
         None,
@@ -1549,14 +1573,25 @@
         None,
         (
             "Sets the amount of money the player is carrying, clamping the value to the"
             " range [0, MAX_MONEY_CARRIED].\n\nr0: new value"
         ),
     )
 
+    AddMoneyCarried = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds the amount of money to the player's current amount of money. Just"
+            " calls\nSetMoneyCarried with the current money + money gained.\n\nr0:"
+            " money gained (can be negative)"
+        ),
+    )
+
     GetCurrentBagCapacity = Symbol(
         [0xEE2C],
         [0x200EE2C],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: bag capacity",
     )
 
@@ -1577,15 +1612,18 @@
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: # items",
     )
 
     CountNbItemsOfTypeInBag = Symbol(
         [0xEEF4],
         [0x200EEF4],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: count",
+        (
+            "Returns the number of items of the given kind in the bag\n\nr0: item"
+            " ID\nreturn: count"
+        ),
     )
 
     CountItemTypeInBag = Symbol(
         [0xEF30],
         [0x200EF30],
         None,
         (
@@ -1806,14 +1844,24 @@
     ScriptSpecialProcess0x39 = Symbol(
         [0xFDFC],
         [0x200FDFC],
         None,
         "Implements SPECIAL_PROC_0x39 (see ScriptSpecialProcessCall).\n\nreturn: bool",
     )
 
+    CountNbItemsOfTypeInStorage = Symbol(
+        [0xFF50],
+        [0x200FF50],
+        None,
+        (
+            "Returns the number of items of the given kind in the storage\n\nr0: item"
+            " ID\nreturn: count"
+        ),
+    )
+
     CountItemTypeInStorage = Symbol(
         [0xFF8C],
         [0x200FF8C],
         None,
         (
             "Implements SPECIAL_PROC_COUNT_ITEM_TYPE_IN_STORAGE (see"
             " ScriptSpecialProcessCall).\n\nr0: pointer to an owned_item\nreturn:"
@@ -2675,38 +2723,62 @@
     )
 
     DeleteWanTableEntry = Symbol(
         [0x1D278],
         [0x201D278],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
+            "Always delete an entry if the file is allocated externally"
+            " (file_externally_allocated is set), otherwise, decrease the reference"
+            " counter. If it reach 0, delete the sprite.\n\nr0: wan_table_ptr\nr1:"
             " wan_id"
         ),
     )
 
+    AllocateWanTableEntry = Symbol(
+        [0x1D2E0],
+        [0x201D2E0],
+        None,
+        (
+            "Return the identifier to a free wan table entry (-1 if none are"
+            " avalaible). The entry is zeroed.\n\nr0: wan_table_ptr\nreturn: the entry"
+            " id in wan_table"
+        ),
+    )
+
     FindWanTableEntry = Symbol(
         [0x1D370],
         [0x201D370],
         None,
         (
-            "Appears to search in the given table (in practice always seems to be"
+            "Search in the given table (in practice always seems to be"
             " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
             " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
             " if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         [0x1D3D0],
         [0x201D3D0],
         None,
         (
-            "wan_id = -1 if it is not loaded\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: wan_table_ptr\nr1: bin_file_id\nr2: file_id\nreturn: wan_id"
+            "Look up a sprite with the provided pack_id and file_index in the wan"
+            " table.\n\nr0: wan_table_ptr\nr1: pack_id\nr2: file_index\nreturn: sprite"
+            " id in the wan table, -1 if not found"
+        ),
+    )
+
+    InitWanTable = Symbol(
+        [0x1D458],
+        [0x201D458],
+        None,
+        (
+            "Initialize the input WAN table with 0x60 free entries (it needs a length"
+            " of 0x1510 bytes)\n\nr0: wan_table_ptr"
         ),
     )
 
     LoadWanTableEntry = Symbol(
         [0x1D478],
         [0x201D478],
         None,
@@ -2714,14 +2786,40 @@
             "Appears to load data from the given file (in practice always seems to be"
             " animation data), using previously loaded data in the given table (see"
             " FindWanTableEntry) if possible.\n\nr0: table pointer\nr1: file name\nr2:"
             " flags\nreturn: table index of the loaded data"
         ),
     )
 
+    LoadWanTableEntryFromPack = Symbol(
+        [0x1D520],
+        [0x201D520],
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3: allocation"
+            " flags\nstack[0]: compressed\nreturn: the entry id in wan_table"
+        ),
+    )
+
+    LoadWanTableEntryFromPackUseProvidedMemory = Symbol(
+        [0x1D62C],
+        [0x201D62C],
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite into the"
+            " provided memory area. Mark the sprite as externally allocated.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3:"
+            " sprite_storage_ptr\nstack[0]: compressed\nreturn: the entry id in"
+            " wan_table"
+        ),
+    )
+
     ReplaceWanFromBinFile = Symbol(
         [0x1D720],
         [0x201D720],
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
             " wan_id\nr2: bin_file_id\nr3: file_id\nstack[0]: compressed"
@@ -2980,14 +3078,30 @@
         [0x245C0], [0x20245C0], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetStringPower = Symbol(
         [0x24688], [0x2024688], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    GetDungeonResultString = Symbol(
+        [0x252A4],
+        [0x20252A4],
+        None,
+        (
+            "Returns a string containing some information to be used when displaying"
+            " the dungeon results screen.\n\nThe exact string returned depends on the"
+            " value of r0:\n0: Name of the move that fainted the leader. Empty string"
+            " if the leader didn't faint.\n1-3: Seems to always result in an empty"
+            " string.\n4: Name of the pokémon that fainted the leader, or name of the"
+            " leader if the leader didn't faint.\n5: Name of the fainted leader. Empty"
+            " string if the leader didn't faint.\n\nr0: String to return\nreturn:"
+            " Pointer to resulting string"
+        ),
+    )
+
     SetQuestionMarks = Symbol(
         [0x253B0],
         [0x20253B0],
         None,
         (
             "Fills the buffer with the string '???'\n\nNote: unverified, ported from"
             " Irdkwia's notes\n\nr0: buffer"
@@ -3313,15 +3427,15 @@
 
     IsMenuOptionActive = Symbol(
         [0x32768],
         [0x2032768],
         None,
         (
             "Called whenever a menu option is selected. Returns whether the option is"
-            " active or not.\n\nr0: ?\nReturn: True if the menu option is enabled,"
+            " active or not.\n\nr0: ?\nreturn: True if the menu option is enabled,"
             " false otherwise."
         ),
     )
 
     ShowKeyboard = Symbol(
         [0x36AE4],
         [0x2036AE4],
@@ -3705,14 +3819,24 @@
         None,
         (
             "Gets the special episode type from the SPECIAL_EPISODE_TYPE script"
             " variable.\n\nreturn: special episode type"
         ),
     )
 
+    GetExecuteSpecialEpisodeType = Symbol(
+        [0x4CC70],
+        [0x204CC70],
+        None,
+        (
+            "Gets the special episode type from the EXECUTE_SPECIAL_EPISODE_TYPE script"
+            " variable.\n\nreturn: special episode type"
+        ),
+    )
+
     HasPlayedOldGame = Symbol(
         [0x4CDA8],
         [0x204CDA8],
         None,
         "Returns the value of the VAR_PLAY_OLD_GAME script variable.\n\nreturn: bool",
     )
 
@@ -3775,21 +3899,21 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: dungeon ID\nr1:"
             " bit_value"
         ),
     )
 
-    CheckDungeonOpen = Symbol(
+    GetDungeonMode = Symbol(
         [0x4D2D4],
         [0x204D2D4],
         None,
         (
-            "Related to dungeon open list\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: dungeon ID\nreturn: status code?"
+            "Returns the mode of the specified dungeon\n\nr0: Dungeon ID\nreturn:"
+            " Dungeon mode"
         ),
     )
 
     GlobalProgressAlloc = Symbol(
         [0x4D440],
         [0x204D440],
         None,
@@ -4002,14 +4126,59 @@
         (
             "If buffer_portrait is null, it only checks if it exists\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: portrait box pointer\nr1:"
             " buffer_portrait\nreturn: exists"
         ),
     )
 
+    SetEnterDungeon = Symbol(
+        [0x4EC84],
+        [0x204EC84],
+        None,
+        (
+            "Used to set the dungeon that will be accessed when switching from ground"
+            " to dungeon mode.\n\nr0: Dungeon ID"
+        ),
+    )
+
+    InitDungeonInit = Symbol(
+        [0x4ED94],
+        [0x204ED94],
+        None,
+        (
+            "Initializes the dungeon_init struct before entering a dungeon.\n\nr0:"
+            " [output] Pointer to the struct to init\nr1: Dungeon ID"
+        ),
+    )
+
+    IsNoLossPenaltyDungeon = Symbol(
+        [0x4F318],
+        [0x204F318],
+        None,
+        (
+            "Returns true if the specified dungeon shouldn't have a loss penalty.\n\nIf"
+            " true you won't lose your money and items upon fainting. Also used to"
+            " initialize dungeon_init::skip_faint_animation_flag.\n\nReturns: True for"
+            " DUNGEON_CRYSTAL_LAKE and DUNGEON_5TH_STATION_CLEARING, as well as for"
+            " DUNGEON_DEEP_STAR_CAVE_TEAM_ROGUE if the ground variable SIDE01_BOSS2ND"
+            " is 0; false otherwise."
+        ),
+    )
+
+    CheckMissionRestrictions = Symbol(
+        [0x4F6FC],
+        [0x204F6FC],
+        None,
+        (
+            "Seems to be used to check if you have any missions that have unmet"
+            " restrictions when trying to access a dungeon.\n\nr0: ?\nreturn: (?) Seems"
+            " to be composed of multiple bitflags."
+        ),
+    )
+
     GetNbFloors = Symbol(
         [0x4F8B4],
         [0x204F8B4],
         None,
         (
             "Returns the number of floors of the given dungeon.\n\nThe result is"
             " hardcoded for certain dungeons, such as dojo mazes.\n\nr0: Dungeon"
@@ -4071,19 +4240,75 @@
         (
             "Given a dungeon ID and a floor number, returns a struct with the"
             " corresponding dungeon group and floor number in that group.\n\nThe"
             " function normally uses the data in mappa_s.bin to calculate the result,"
             " but there's some dungeons (such as dojo mazes) that have hardcoded return"
             " values.\n\nIrdkwia's notes:\n  [r1]: dungeon_id\n  [r1+1]:"
             " dungeon_floor_id\n  [r0]: group_id\n  [r0+1]: group_floor_id\n\nr0:"
-            " (output) Struct containing the dungeon group and floor group\nr1: Struct"
+            " [output] Struct containing the dungeon group and floor group\nr1: Struct"
             " containing the dungeon ID and floor number"
         ),
     )
 
+    GetMissionRank = Symbol(
+        [0x4FB4C],
+        [0x204FB4C],
+        None,
+        (
+            "Gets the mission rank for the given dungeon and floor.\n\nIf the dungeon"
+            " ID is >= DUNGEON_NORMAL_FLY_MAZE or the group of the dungeon is >"
+            " DGROUP_DUMMY_0x63, returns MISSION_RANK_E.\n\nr0: Dungeon and"
+            " floor\nreturn: Mission rank"
+        ),
+    )
+
+    GetOutlawLevel = Symbol(
+        [0x4FBC4],
+        [0x204FBC4],
+        None,
+        (
+            "Gets the level that should be used for outlaws for the given dungeon and"
+            " floor\n\nr0: Dungeon and floor\nreturn: Outlaw level"
+        ),
+    )
+
+    GetOutlawLeaderLevel = Symbol(
+        [0x4FBE0],
+        [0x204FBE0],
+        None,
+        (
+            "Gets the level that should be used for team leader outlaws for the given"
+            " dungeon and floor. Identical to GetOutlawLevel.\n\nr0: Dungeon and"
+            " floor\nreturn: Outlaw leader level"
+        ),
+    )
+
+    GetOutlawMinionLevel = Symbol(
+        [0x4FBFC],
+        [0x204FBFC],
+        None,
+        (
+            "Gets the level that should be used for minion outlaws for the given"
+            " dungeon and floor.\n\nr0: Dungeon and floor\nreturn: Outlaw minion level"
+        ),
+    )
+
+    AddGuestMonster = Symbol(
+        [0x4FC18],
+        [0x204FC18],
+        None,
+        (
+            "Adds a guest monster to the active team\n\nr0: dungeon_init struct for the"
+            " dungeon that is about to be entered\nr1: Number of the guest monster to"
+            " add. Used when more than one monster is added.\nr2: Pointer to the guest"
+            " monster entry to add to the team (usually located within"
+            " GUEST_MONSTER_DATA)"
+        ),
+    )
+
     GetGroundNameId = Symbol(
         [0x4FC90], [0x204FC90], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetAdventureLogStructLocation = Symbol(
         [0x4FD5C],
         [0x204FD5C],
@@ -5181,14 +5406,24 @@
     LoadM2nAndN2m = Symbol(
         [0x52F0C],
         [0x2052F0C],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    GuestMonsterToGroundMonster = Symbol(
+        [0x531CC],
+        [0x20531CC],
+        None,
+        (
+            "Inits a ground_monster entry with the given guest_monster struct.\n\nr0:"
+            " [output] ground_monster struct to init\nr1: guest_monster struct to use"
+        ),
+    )
+
     StrcmpMonsterName = Symbol(
         [0x5332C],
         [0x205332C],
         None,
         (
             "Checks if the string_buffer matches the name of the species\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: string_buffer\nr1: monster"
@@ -5760,15 +5995,15 @@
         [0x59080],
         [0x2059080],
         None,
         (
             "Determines the list of IQ skills that a given monster can learn given its"
             " IQ value.\n\nThe list of skills is written in the array specified in r0."
             " The array has 69 slots in total. Unused slots are set to 0.\n\nr0:"
-            " (output) Array where the list of skills will be written\nr1: Monster"
+            " [output] Array where the list of skills will be written\nr1: Monster"
             " species\nr2: Monster IQ\nreturn: Amount of skills written to the output"
             " array"
         ),
     )
 
     DisableIqSkill = Symbol(
         [0x59120],
@@ -6215,14 +6450,29 @@
         (
             "Converts an index in DUNGEON_SWAP_ID_TABLE to the corresponding dungeon"
             " ID, or DUNGEON_DUMMY_0xFF if the index is -1.\n\nr0: index\nreturn:"
             " dungeon ID"
         ),
     )
 
+    GetDungeonModeSpecial = Symbol(
+        [0x6AB04],
+        [0x206AB04],
+        None,
+        (
+            "Returns the status of the given dungeon, with some modifications.\n\nIf"
+            " the dungeon ID is DUNGEON_BEACH, returns DMODE_REQUEST.\nIf it's"
+            " DUNGEON_JOINED_AT_UNKNOWN, returns DMODE_OPEN_AND_REQUEST.\nIf it's >="
+            " DUNGEON_NORMAL_FLY_MAZE and <= DUNGEON_DOJO_0xD3, returns"
+            " DMODE_OPEN_AND_REQUEST.\nElse, calls GetDungeonMode and returns"
+            " DMODE_REQUEST if the dungeon has been cleared, or DMODE_OPEN if it's"
+            " not.\n\nr0: Dungeon ID\nreturn: Dungeon mode"
+        ),
+    )
+
     ResumeBgm = Symbol(
         [0x6DD54],
         [0x206DD54],
         None,
         "Uncertain.\n\nNote: unverified, ported from Irdkwia's notes",
     )
 
@@ -6233,14 +6483,94 @@
     UpdateChannels = Symbol(
         [0x74824],
         [0x2074824],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    ClearIrqFlag = Symbol(
+        [0x7BB68],
+        [0x207BB68],
+        None,
+        (
+            "Enables processor interrupts by clearing the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were disabled, 0x0 if they were already enabled)"
+        ),
+    )
+
+    EnableIrqFlag = Symbol(
+        [0x7BB7C],
+        [0x207BB7C],
+        None,
+        (
+            "Disables processor interrupts by setting the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were already disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    SetIrqFlag = Symbol(
+        [0x7BB90],
+        [0x207BB90],
+        None,
+        (
+            "Sets the value of the processor's interrupt flag according to the"
+            " specified parameter.\n\nr0: Value to set the flag to (0x80 to set it,"
+            " which disables interrupts; 0x0 to unset it, which enables"
+            " interrupts)\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts were"
+            " disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    EnableIrqFiqFlags = Symbol(
+        [0x7BBA8],
+        [0x207BBA8],
+        None,
+        (
+            "Disables processor all interrupts (both standard and fast) by setting the"
+            " i and f flags in the program status register (cpsr).\n\nreturn: Old value"
+            " of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    SetIrqFiqFlags = Symbol(
+        [0x7BBBC],
+        [0x207BBBC],
+        None,
+        (
+            "Sets the value of the processor's interrupt flags (i and f) according to"
+            " the specified parameter.\n\nr0: Value to set the flags to (0xC0 to set"
+            " both flags, 0x80 to set the i flag and clear the f flag, 0x40 to set the"
+            " f flag and clear the i flag and 0x0 to clear both flags)\nreturn: Old"
+            " value of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    GetIrqFlag = Symbol(
+        [0x7BBD4],
+        [0x207BBD4],
+        None,
+        (
+            "Gets the current value of the processor's interrupt request (i)"
+            " flag\n\nreturn: cpsr & 0x80 (0x80 if interrupts are disabled, 0x0 if they"
+            " are enabled)"
+        ),
+    )
+
+    WaitForever2 = Symbol(
+        [0x7BFB8],
+        [0x207BFB8],
+        None,
+        (
+            "Calls EnableIrqFlag and WaitForInterrupt in an infinite loop.\n\nThis is"
+            " called on fatal errors to hang the program indefinitely.\n\nNo params."
+        ),
+    )
+
     WaitForInterrupt = Symbol(
         [0x7BFC8],
         [0x207BFC8],
         None,
         (
             "Presumably blocks until the program receives an interrupt.\n\nThis just"
             " calls (in Ghidra terminology) coproc_moveto_Wait_for_interrupt(0). See"
@@ -12912,14 +13242,24 @@
         0x4,
         (
             "The multiplier for damage from the Air Blade (1.5), as a binary"
             " fixed-point number (8 fraction bits)"
         ),
     )
 
+    KECLEON_SHOP_BOOST_CHANCE_MULTIPLIER = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The boosted kecleon shop spawn chance multiplier (~1.2) as a binary"
+            " fixed-point number (8 fraction bits)."
+        ),
+    )
+
     HIDDEN_STAIRS_SPAWN_CHANCE_MULTIPLIER = Symbol(
         [0x7DE8],
         [0x22C51A8],
         0x4,
         (
             "The hidden stairs spawn chance multiplier (~1.2) as a binary fixed-point"
             " number (8 fraction bits), if applicable. See"
@@ -13600,16 +13940,18 @@
     )
 
     LoadBackgroundAttributes = Symbol(
         [0xF900],
         [0x22EC480],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: [output]"
-            " bg_attr_str\nr1: bg_id"
+            "Open and read an entry from the MAP_BG/bg_list.dat\n\nDocumentation on"
+            " this format can be found"
+            " here:\nhttps://github.com/SkyTemple/skytemple-files/tree/55b3017631a8a1b0f106111ef91a901dc394c6df/skytemple_files/graphics/bg_list_dat\n\nr0:"
+            " [output] The entry\nr1: background ID"
         ),
     )
 
     LoadMapType10 = Symbol(
         [0x10AE4],
         [0x22ED664],
         None,
@@ -13712,14 +14054,24 @@
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
             " characters printed, excluding the null-terminator"
         ),
     )
 
+    GetExclusiveItemRequirements = Symbol(
+        [0x2ED54],
+        [0x230B8D4],
+        None,
+        (
+            "Used to calculate the items required to get a certain exclusive item in"
+            " the swap shop.\n\nr0: ?\nr1: ?"
+        ),
+    )
+
     StatusUpdate = Symbol(
         [0x378F8],
         [0x2314478],
         None,
         (
             "Implements SPECIAL_PROC_STATUS_UPDATE (see"
             " ScriptSpecialProcessCall).\n\nNo params."
@@ -13878,14 +14230,21 @@
         ),
     )
 
     UNIONALL_RAM_ADDRESS = Symbol([0x48C64], [0x23257E4], None, "[Runtime]")
 
     GROUND_STATE_MAP = Symbol([0x48C80], [0x2325800], None, "[Runtime]")
 
+    GROUND_STATE_WEATHER = Symbol(
+        [0x48C8C],
+        [0x232580C],
+        None,
+        "[Runtime] Same structure format as GROUND_STATE_MAP",
+    )
+
     GROUND_STATE_PTRS = Symbol(
         [0x48CB4],
         [0x2325834],
         0x18,
         (
             "Host pointers to multiple structure used for performing an overworld"
             " scene\n\ntype: struct main_ground_data"
@@ -15843,24 +16202,81 @@
     FadeToBlack = Symbol(
         [0x4728],
         [0x22E12A8],
         None,
         "Fades the screen to black across several frames.\n\nNo params.",
     )
 
+    CheckTouchscreenArea = Symbol(
+        [0x4A78],
+        [0x22E15F8],
+        None,
+        (
+            "Checks if the currently pressed touchscreen position is within the"
+            " specified area.\n\nr0: Area lower X coordinate\nr1: Area lower Y"
+            " coordinate\nr2: Area upper X coordinate\nr3: Area upper Y"
+            " coordinate\nreturn: True if the specified area contains the currently"
+            " pressed touchscreen position, false otherwise."
+        ),
+    )
+
+    GetTrapInfo = Symbol(
+        [0x53C8],
+        [0x22E1F48],
+        None,
+        (
+            "Given a trap entity, returns the pointer to the trap info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Trap data pointer"
+        ),
+    )
+
+    GetItemInfo = Symbol(
+        [0x53D0],
+        [0x22E1F50],
+        None,
+        (
+            "Given an item entity, returns the pointer to the item info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Item data pointer"
+        ),
+    )
+
     GetTileAtEntity = Symbol(
         [0x53E8],
         [0x22E1F68],
         None,
         (
             "Returns a pointer to the tile where an entity is located.\n\nr0: pointer"
             " to entity\nreturns: pointer to tile"
         ),
     )
 
+    UpdateEntityPixelPos = Symbol(
+        [0x5800],
+        [0x22E2380],
+        None,
+        (
+            "Updates an entity's pixel_pos field using the specified pixel_position"
+            " struct, or its own pos field if it's null.\n\nr0: Entity pointer\nr1:"
+            " Pixel position to use, or null to use the entity's own position"
+        ),
+    )
+
+    CreateEnemyEntity = Symbol(
+        [0x5E80],
+        [0x22E2A00],
+        None,
+        (
+            "Creates and initializes the entity struct of a newly spawned enemy"
+            " monster. Fails if there's 16 enemies on the floor already.\n\nIt could"
+            " also be used to spawn fixed room allies, since those share their slots on"
+            " the entity list.\n\nr0: Monster ID\nreturn: Pointer to the newly"
+            " initialized entity, or null if the entity couldn't be initialized"
+        ),
+    )
+
     SpawnTrap = Symbol(
         [0x6020],
         [0x22E2BA0],
         None,
         (
             "Spawns a trap on the floor. Fails if there are more than 64 traps already"
             " on the floor.\n\nThis modifies the appropriate fields on the dungeon"
@@ -15880,35 +16296,46 @@
             " items already on the floor.\n\nThis initializes a new entry in the entity"
             " table and points it to the corresponding slot in the item info"
             " list.\n\nr0: position\nreturn: entity pointer for the newly added item,"
             " or null on failure"
         ),
     )
 
-    ShouldDisplayEntityMessages = Symbol(
+    ShouldMinimapDisplayEntity = Symbol(
+        [0x6258],
+        [0x22E2DD8],
+        None,
+        (
+            "Checks if a given entity should be displayed on the minimap\n\nr0: Entity"
+            " pointer\nreturn: True if the entity should be displayed on the minimap"
+        ),
+    )
+
+    ShouldDisplayEntity = Symbol(
         [0x6334],
         [0x22E2EB4],
         None,
         (
-            "Checks if messages that involve a certain entity should be displayed or"
-            " suppressed.\n\nFor example, it returns false if the entity is an"
-            " invisible enemy.\n\nr0: Entity pointer\nr1: ?\nreturn: True if messages"
-            " involving the entity should be displayed, false if they should be"
-            " suppressed."
+            "Checks if an entity should be displayed or not.\n\nFor example, it returns"
+            " false if the entity is an invisible enemy.\nAlso used to determine if"
+            " messages that involve a certain entity should be displayed or"
+            " suppressed.\n\nr0: Entity pointer\nr1: (?) Seems to be 1 for monsters and"
+            " 0 for items.\nreturn: True if the entity and its associated messages"
+            " should be displayed, false if they shouldn't."
         ),
     )
 
-    ShouldDisplayEntityMessagesWrapper = Symbol(
+    ShouldDisplayEntityWrapper = Symbol(
         [0x64EC],
         [0x22E306C],
         None,
         (
-            "Calls ShouldDisplayEntityMessages with r1 = 0\n\nr0: Entity"
-            " pointer\nreturn: True if messages involving the entity should be"
-            " displayed, false if they should be suppressed."
+            "Calls ShouldDisplayEntity with r1 = 0\n\nr0: Entity pointer\nreturn: True"
+            " if the entity and its associated messages should be displayed, false if"
+            " they shouldn't."
         ),
     )
 
     CanSeeTarget = Symbol(
         [0x650C],
         [0x22E308C],
         None,
@@ -16056,28 +16483,54 @@
         (
             "Returns dungeon::display_data::visibility_range. If the visibility range"
             " is 0, returns 2 instead.\n\nreturn: Visibility range of the current"
             " floor, or 2 if the visibility is 0."
         ),
     )
 
-    PlayEffectAnimation = Symbol(
+    PlayEffectAnimationEntity = Symbol(
         [0x7414],
         [0x22E3F94],
         None,
         (
             "Just a guess. This appears to be paired often with"
             " GetEffectAnimationField0x19, and also has calls AnimationHasMoreFrames in"
             " a loop alongside AdvanceFrame(66) calls.\n\nThe third parameter skips the"
             " loop entirely. It seems like in this case the function might just preload"
-            " some animation frames for later use??\n\nr0: entity pointer\nr1: ?\nr2:"
-            " appears to be a flag for actually running the animation now? If this is"
-            " 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn: status"
-            " code, or maybe the number of frames or something? Either way, -1 seems to"
-            " indicate the animation being finished or something?"
+            " some animation frames for later use??\n\nr0: entity pointer\nr1: Effect"
+            " ID\nr2: appears to be a flag for actually running the animation now? If"
+            " this is 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn:"
+            " status code, or maybe the number of frames or something? Either way, -1"
+            " seems to indicate the animation being finished or something?"
+        ),
+    )
+
+    PlayEffectAnimationPos = Symbol(
+        [0x760C],
+        [0x22E418C],
+        None,
+        (
+            "Takes a position struct in r0 and converts it to a pixel position struct"
+            " before calling PlayEffectAnimationPixelPos\n\nr0: Position where the"
+            " effect should be played\nr1: Effect ID\nr2: Unknown flag (same as the one"
+            " in PlayEffectAnimationEntity)\nreturn: Result of call to"
+            " PlayEffectAnimationPixelPos"
+        ),
+    )
+
+    PlayEffectAnimationPixelPos = Symbol(
+        [0x7650],
+        [0x22E41D0],
+        None,
+        (
+            "Seems like a variant of PlayEffectAnimationEntity that uses pixel"
+            " coordinates as its first parameter instead of an entity pointer.\n\nr0:"
+            " Pixel position where the effect should be played\nr1: Effect ID\nr2:"
+            " Unknown flag (same as the one in PlayEffectAnimationEntity)\nreturn: Same"
+            " as PlayEffectAnimationEntity"
         ),
     )
 
     UpdateStatusIconFlags = Symbol(
         [0x78E4],
         [0x22E4464],
         None,
@@ -16165,15 +16618,15 @@
         [0x22E8610],
         None,
         (
             "Copies all entries in the floor's monster spawn list that have a sprite"
             " size >= 6 to the specified buffer.\n\nThe parameter in r1 can be used to"
             " specify how many entries are already present in the buffer. Entries added"
             " by this function will be placed after those, and the total returned in r1"
-            " will account for existing entries as well.\n\nr0: (output) Buffer where"
+            " will account for existing entries as well.\n\nr0: [output] Buffer where"
             " the result will be stored\nr1: Current amount of entries in the"
             " buffer\nreturn: New amount of entries in the buffer"
         ),
     )
 
     IsOnMonsterSpawnList = Symbol(
         [0xBB7C],
@@ -16545,14 +16998,26 @@
             " the effect of the Switcher Orb). \n\nThe function checks for the Suction"
             " Cups ability for both the user and the target, and for the Mold Breaker"
             " ability on the user.\n\nr0: pointer to user entity\nr1: pointer to target"
             " entity"
         ),
     )
 
+    SetLeaderActionFields = Symbol(
+        [0xF1F8],
+        [0x22EBD78],
+        None,
+        (
+            "Sets the leader's monster::action::action_id to the specified"
+            " value.\n\nAlso sets monster::action::action_use_idx and"
+            " monster::action::field_0xA to 0, as well as monster::action::field_0x10"
+            " and monster::action::field_0x12 to -1.\n\nr0: ID of the action to set"
+        ),
+    )
+
     ClearMonsterActionFields = Symbol(
         [0xF224],
         [0x22EBDA4],
         None,
         (
             "Clears the fields related to AI in the monster's data struct, setting them"
             " all to 0.\nSpecifically, monster::action::action_id,"
@@ -16632,14 +17097,27 @@
         (
             "Sets a monster's action to action::ACTION_REGULAR_ATTACK, with a specified"
             " direction.\n\nr0: Pointer to the monster's action field\nr1: Direction in"
             " which to use the move. Gets stored in monster::action::direction."
         ),
     )
 
+    SetActionUseMovePlayer = Symbol(
+        [0xFAC8],
+        [0x22EC648],
+        None,
+        (
+            "Sets a monster's action to action::ACTION_USE_MOVE_PLAYER, with a"
+            " specified monster and move index.\n\nr0: Pointer to the monster's action"
+            " field\nr1: Index of the monster that is using the move on the entity"
+            " list. Gets stored in monster::action::action_use_idx.\nr2: Index of the"
+            " move to use (0-3). Gets stored in monster::action::field_0xA."
+        ),
+    )
+
     SetActionUseMoveAi = Symbol(
         [0xFAEC],
         [0x22EC66C],
         None,
         (
             "Sets a monster's action to action::ACTION_USE_MOVE_AI, with a specified"
             " direction and move index.\n\nr0: Pointer to the monster's action"
@@ -16786,14 +17264,169 @@
             "If the flag for a trapper trap is set, handles spawning a trap based upon"
             " the\ninformation inside the dungeon struct. Uses the entity for logging a"
             " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
             " true if a trap was spawned succesfully"
         ),
     )
 
+    TryTriggerTrap = Symbol(
+        [0x11DD0],
+        [0x22EE950],
+        None,
+        (
+            "Called whenever a monster steps on a trap.\n\nThe function will try to"
+            " trigger it. Nothing will happen if the pokémon has the same team as the"
+            " trap. The attempt to trigger the trap can also fail due to IQ skills, due"
+            " to the trap failing to work (random chance), etc.\n\nr0: Entity who"
+            " stepped on the trap\nr1: Trap position\nr2: ?\nr3: ?"
+        ),
+    )
+
+    ApplyMudTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly lowers attack, special attack, defense, or special defense of the"
+            " defender by 3 stages.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer"
+        ),
+    )
+
+    ApplyStickyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to make something in the bag"
+            " sticky. Otherwise, try to make the item the monster is holding"
+            " sticky.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyGrimyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to turn food items in the"
+            " toolbox into\ngrimy food. Otherwise, try to make the food item the"
+            " monster is holding grimy food.\n\nr0: attacker entity pointer\nr1:"
+            " defender entity pointer"
+        ),
+    )
+
+    ApplyPitfallTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, end the current floor unless it has a"
+            " rescue point.\nOtherwise, make the entity faint and ignore reviver seeds."
+            " If not called by a random\ntrap, break the grate on the pitfall"
+            " trap.\n\nr0: attacker entity pointer\nr1: defender entity pointer\nr2:"
+            " tile pointer\nr3: bool caused by random trap"
+        ),
+    )
+
+    ApplySummonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly spawns 2-4 enemy monsters around the position. The entity is only"
+            " used for\nlogging messages.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyPpZeroTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the PP of one of the defender's moves to 0.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyPokemonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Turns item in the same room as the tile at the position (usually just the"
+            " entities's\nposition) into monsters. If the position is in a hallway,"
+            " convert items in a 3x3 area\ncentered on the position into"
+            " monsters.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTripTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to drop the defender's item and places it on the floor.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyToxicSpikesTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to inflict 10 damage on the defender and then tries to poison"
+            " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyRandomTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Selects a random trap that isn't a wonder tile and isn't a random trap and"
+            " calls\nApplyTrapEffect on all monsters that is different from the trap's"
+            " team.\n\nr0: Triggered trap\nr1: User\nr2: Target, normally same as"
+            " user\nr3: Tile that contains the trap\nstack[0]: position"
+        ),
+    )
+
+    ApplyGrudgeTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Spawns several monsters around the position and gives all monsters on the"
+            " floor the\ngrudge status condition.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTrapEffect = Symbol(
+        [0x12F88],
+        [0x22EFB08],
+        None,
+        (
+            "Performs the effect of a triggered trap.\n\nThe trap's animation happens"
+            " before this function is called.\n\nr0: Triggered trap\nr1: User\nr2:"
+            " Target, normally same as user\nr3: Tile that contains the trap\nstack[0]:"
+            " position\nstack[1]: trap ID\nstack[2]: bool caused by random"
+            " trap\nreturn: True if the trap should be destroyed after the effect is"
+            " applied"
+        ),
+    )
+
+    RevealTrapsNearby = Symbol(
+        None,
+        None,
+        None,
+        "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x138A0],
         [0x22F0420],
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16817,28 +17450,63 @@
         None,
         (
             "Returns a pointer to the action data of the current leader (field 0x4A on"
             " its monster struct).\n\nNo params."
         ),
     )
 
+    GetEntityTouchscreenArea = Symbol(
+        [0x149E0],
+        [0x22F1560],
+        None,
+        (
+            "Returns the area on the touchscreen that contains the sprite of the"
+            " specified entity\n\nr0: Entity pointer\nr1: [output] struct where the"
+            " result should be written"
+        ),
+    )
+
     SetLeaderAction = Symbol(
         [0x14D10],
         [0x22F1890],
         None,
         (
             "Sets the leader's action field depending on the inputs given by the"
             " player.\n\nThis function also accounts for other special situations that"
             " can force a certain action, such as when the leader is running. The"
             " function also takes care of opening the main menu when X is pressed.\nThe"
             " function generally doesn't return until the player has an action"
             " set.\n\nNo params."
         ),
     )
 
+    ShouldLeaderKeepRunning = Symbol(
+        [0x16EC4],
+        [0x22F3A44],
+        None,
+        (
+            "Determines if the leader should keep running. Returns false if the leader"
+            " bumps into something, or if an action that should stop the leader takes"
+            " place.\n\nreturn: True if the leader should keep running, false if it"
+            " should stop."
+        ),
+    )
+
+    CheckLeaderTile = Symbol(
+        [0x1746C],
+        [0x22F3FEC],
+        None,
+        (
+            "Checks the tile the leader just stepped on and performs any required"
+            " actions, such as picking up items, triggering traps, etc.\n\nContains a"
+            " switch that checks the type of the tile the leader just stepped on.\n\nNo"
+            " params."
+        ),
+    )
+
     ChangeLeader = Symbol(
         [0x17770],
         [0x22F42F0],
         None,
         (
             "Tries to change the current leader to the monster specified by"
             " dungeon::new_leader.\n\nAccounts for situations that can prevent changing"
@@ -16981,14 +17649,25 @@
         (
             "Handles a fainted pokémon (reviving does not count as fainting).\n\nr0:"
             " Fainted entity\nr1: Damage source (move ID or greater than the max move"
             " id for other causes)\nr2: Entity responsible of the fainting"
         ),
     )
 
+    MoveMonsterToPos = Symbol(
+        [0x1C47C],
+        [0x22F8FFC],
+        None,
+        (
+            "Moves a monster to the target position. Used both for regular movement and"
+            " special movement (like teleportation).\n\nr0: Entity pointer\nr1: X"
+            " target position\nr2: Y target position\nr3: ?"
+        ),
+    )
+
     UpdateAiTargetPos = Symbol(
         [0x1CFD0],
         [0x22F9B50],
         None,
         (
             "Given a monster, updates its target_pos field based on its current"
             " position and the direction in which it plans to attack.\n\nr0: Entity"
@@ -17133,14 +17812,24 @@
             "Restores PP for all moves, clears flags move::f_consume_2_pp,"
             " move::flags2_unk5 and move::flags2_unk7, and sets flag"
             " move::f_consume_pp.\nCalled when a monster is revived.\n\nr0: pointer to"
             " entity whose moves will be restored"
         ),
     )
 
+    BoostIQ = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's IQ.\n\nr0: monster entity pointer\nr1: iq"
+            " boost\nr2: bool suppress logs"
+        ),
+    )
+
     ShouldMonsterHeadToStairs = Symbol(
         [0x1E2BC],
         [0x22FAE3C],
         None,
         (
             "Checks if a given monster should try to reach the stairs when controlled"
             " by the AI\n\nr0: Entity pointer\nreturn: True if the monster should try"
@@ -17157,14 +17846,28 @@
             " dungeon::mew_cannot_spawn or the second parameter are true.\n\nCalled"
             " before spawning an enemy, appears to be checking if Mew can spawn on the"
             " current floor.\n\nr0: monster id\nr1: return false if the monster id is"
             " Mew\nreturn: bool"
         ),
     )
 
+    TryEndStatusWithAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if any of the defender's active abilities would end one of their"
+            " current status\nconditions. For example, if the ability Own Tempo will"
+            " stop confusion.\n\nCalled after changing a monster's ability with skill"
+            " swap, role play, or trace to\nremove statuses the monster should no"
+            " longer be affected by.\n\nr0: attacker entity pointer\nr1: defender"
+            " entity pointer"
+        ),
+    )
+
     ExclusiveItemEffectIsActive = Symbol(
         [
             0x1EB24,
             0x23DD4,
             0x2E8AC,
             0x337A0,
             0x34F44,
@@ -17320,14 +18023,27 @@
             "Checks if a monster does not gain experience.\n\nThis basically just"
             " inverts IsSpecialStoryAlly, with the exception of also checking for the"
             " 'Joined At' field being DUNGEON_CLIENT (is this set for mission"
             " clients?).\n\nr0: monster pointer\nreturn: bool"
         ),
     )
 
+    InitOtherMonsterData = Symbol(
+        [0x1FCD4],
+        [0x22FC854],
+        None,
+        (
+            "Initializes stats, IQ skills and moves for a given monster\n\nMight only"
+            " be used when spawning fixed room monsters.\n\nr0: Entity pointer\nr1:"
+            " Fixed room monster stats index\nr2: Spawn direction? (when calling this"
+            " function while spawning a fixed room monster, this is the parameter value"
+            " associated to the spawn action, after converting it to a direction.)"
+        ),
+    )
+
     SpawnTeam = Symbol(
         [0x20388],
         [0x22FCF08],
         None,
         "Seems to initialize and spawn the team when entering a dungeon.\n\nr0: ?",
     )
 
@@ -17367,20 +18083,32 @@
             " to the struct containing the data of the team member to"
             " initialize\nstack[0]: ?\nstack[1]: ?\nstack[2]: ?\nstack[3]:"
             " ?\nstack[4]: ?"
         ),
     )
 
     InitMonster = Symbol(
+        [0x21850],
+        [0x22FE3D0],
+        None,
+        (
+            "Initializes the monster struct within the provided entity struct.\n\nr0:"
+            " ?\nr1: Pointer to the entity whose monster struct should be"
+            " initialized\nr2: pointer to the entity's spawned_monster_data struct\nr3:"
+            " (?) Pointer to something"
+        ),
+    )
+
+    SubInitMonster = Symbol(
         [0x21C3C],
         [0x22FE7BC],
         None,
         (
-            "Initializes a monster struct.\n\nr0: pointer to monster to initialize\nr1:"
-            " some flag"
+            "Called by InitMonster. Initializes some fields on the monster"
+            " struct.\n\nr0: pointer to monster to initialize\nr1: some flag"
         ),
     )
 
     MarkShopkeeperSpawn = Symbol(
         [0x22014],
         [0x22FEB94],
         None,
@@ -17485,14 +18213,24 @@
         (
             "Returns the number of attacks that a monster can do in one turn (1 or"
             " 2).\n\nChecks for the abilities Swift Swim, Chlorophyll, Unburden, and"
             " for exclusive items.\n\nr0: pointer to entity\nreturns: int"
         ),
     )
 
+    GetMonsterDisplayNameType = Symbol(
+        [0x23FB4],
+        [0x2300B34],
+        None,
+        (
+            "Determines how the name of a monster should be displayed.\n\nr0: Entity"
+            " pointer\nreturn: Display name type"
+        ),
+    )
+
     GetMonsterName = Symbol(
         [0x24010],
         [0x2300B90],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: buffer\nr1: TargetInfo",
     )
 
@@ -17643,14 +18381,39 @@
         None,
         (
             "Checks if a monster has the sleep, nightmare, or napping status.\n\nr0:"
             " entity pointer\nreturn: bool"
         ),
     )
 
+    CanMonsterMoveInDirection = Symbol(
+        [0x24D24],
+        [0x23018A4],
+        None,
+        (
+            "Checks if the given monster can move in the specified direction\n\nReturns"
+            " false if any monster is standing on the target tile\n\nr0: Monster entity"
+            " pointer\nr1: Direction to check\nreturn: bool"
+        ),
+    )
+
+    GetFinalMobilityType = Symbol(
+        [0x24DDC],
+        [0x230195C],
+        None,
+        (
+            "Returns the mobility type of a monster, after accounting for things that"
+            " could affect it (like items or IQ skills)\n\nIf the specified direction"
+            " is DIR_NONE, direction checks are skipped. If it's not,"
+            " MOBILITY_INTANGIBLE is only returned if the direction is not"
+            " diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility type\nr2:"
+            " Direction of mobility\nreturn: Final mobility type"
+        ),
+    )
+
     IsMonsterCornered = Symbol(
         [0x24FC4],
         [0x2301B44],
         None,
         (
             "True if the given monster is cornered (it can't move in any"
             " direction)\n\nr0: Entity pointer\nreturn: True if the monster can't move"
@@ -17678,15 +18441,15 @@
         [0x2301D24],
         None,
         (
             "Checks whether an AI-controlled monster can move in the specified"
             " direction.\nAccounts for walls, other monsters on the target position and"
             " IQ skills that might prevent a monster from moving into a specific"
             " location, such as House Avoider, Trap Avoider or Lava Evader.\n\nr0:"
-            " Entity pointer\nr1: Direction\nr2: (output) True if movement was not"
+            " Entity pointer\nr1: Direction\nr2: [output] True if movement was not"
             " possible because there was another monster on the target tile, false"
             " otherwise.\nreturn: True if the monster can move in the specified"
             " direction, false otherwise."
         ),
     )
 
     ShouldMonsterRunAway = Symbol(
@@ -17706,14 +18469,47 @@
         (
             "Calls ShouldMonsterRunAway and returns its result. It also calls another"
             " function if the result was true.\n\nr0: Entity pointer\nr1: ?\nreturn:"
             " Result of the call to ShouldMonsterRunAway"
         ),
     )
 
+    SafeguardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Safeguard.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: flag to log a message\nreturn:"
+            " bool"
+        ),
+    )
+
+    LeafGuardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is protected by the ability Leaf Guard.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer\nr2: flag to log a"
+            " message\nreturn: bool"
+        ),
+    )
+
+    IsProtectedFromStatDrops = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting their stats dropped"
+            " by the user.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     NoGastroAcidStatus = Symbol(
         [0x25B88],
         [0x2302708],
         None,
         (
             "Checks if a monster does not have the Gastro Acid status.\n\nr0: entity"
             " pointer\nreturn: bool"
@@ -17874,14 +18670,25 @@
             "Updates monster::state_flags and monster::prev_state_flags with new"
             " values.\n\nr0: monster pointer\nr1: bitmask for bits to update\nr2:"
             " whether to set the bits indicated by the mask to 1 or 0\nreturn: whether"
             " or not any of the masked bits changed from the previous state"
         ),
     )
 
+    IsProtectedFromNegativeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting a negative status"
+            " condition.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     AddExpSpecial = Symbol(
         [0x263E8],
         [0x2302F68],
         None,
         (
             "Adds to a monster's experience points, subject to experience boosting"
             " effects.\n\nThis function appears to be called only under special"
@@ -17895,17 +18702,31 @@
     )
 
     EnemyEvolution = Symbol(
         [0x265A8],
         [0x2303128],
         None,
         (
-            "Checks if the specified enemy should evolve because it just defeated an"
-            " ally, and if so, attempts to evolve it.\n\nr0: Pointer to the enemy to"
-            " check"
+            "Checks if any enemies on the floor should evolve and attempts to evolve"
+            " it. The\nentity pointer passed seems to get replaced by a generic"
+            " placeholder entity if the\nentity pointer passed is invalid.\n\nr0:"
+            " entity pointer"
+        ),
+    )
+
+    LevelUpItemEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to level up the the target. Calls LevelUp with a few extra checks"
+            " and messages\nfor using as an item. Used for the Joy Seed and Golden"
+            " Seed.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: number"
+            " of levels\nr3: bool message flag?\nstack[0]: bool show level up dialog"
+            " (for example 'Hey, I leveled up!' with a portrait)?"
         ),
     )
 
     TryDecreaseLevel = Symbol(
         [0x26E34],
         [0x23039B4],
         None,
@@ -17917,27 +18738,31 @@
     )
 
     LevelUp = Symbol(
         [0x26EE8],
         [0x2303A68],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: user entity"
-            " pointer\nr1: target entity pointer\nr2: message flag?\nr3: ?\nreturn:"
-            " success flag?"
+            "Attempts to level up the the target. Fails if the target's level can't be"
+            " raised. The show show level up dialog bool does nothing for monsters not"
+            " on the team.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " bool message flag?\nr3: bool show level up dialog (for example 'Hey, I"
+            " leveled up!' with a portrait)?\nreturn: success flag"
         ),
     )
 
     EvolveMonster = Symbol(
         [0x27B28],
         [0x23046A8],
         None,
         (
-            "Makes the specified monster evolve into the specified species.\n\nr0:"
-            " Pointer to the entity to evolve\nr1: ?\nr2: Species to evolve into"
+            "Makes the specified monster evolve into the specified species. Has a"
+            " special case when\na monster evolves into Ninjask and tries to spawn a"
+            " Shedinja as well.\n\nr0: user entity pointer?\nr1: target pointer to the"
+            " entity to evolve\nr2: Species to evolve into"
         ),
     )
 
     GetSleepAnimationId = Symbol(
         [0x28960],
         [0x23054E0],
         None,
@@ -17959,14 +18784,58 @@
             " example, this delayed display system is used to display multiple monsters"
             " moving at once even though they take turns sequentially.\n\nr0: Pointer"
             " to an entity. Can be null.\nreturns: Seems to be true if there were any"
             " pending actions to display."
         ),
     )
 
+    CheckNonLeaderTile = Symbol(
+        [0x29540],
+        [0x23060C0],
+        None,
+        (
+            "Similar to CheckLeaderTile, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: Entity pointer"
+        ),
+    )
+
+    EndNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Cures the target's negative status conditions. The game rarely (if not"
+            " never) calls\nthis function with the bool to remove the wrapping status"
+            " false.\n\nr0: pointer to user\nr1: pointer to target\nr2: bool play"
+            " animation\nr3: bool log failure message\nstack[0]: bool remove wrapping"
+            " status\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    EndNegativeStatusConditionWrapper = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EndNegativeStatusCondition with remove wrapping status false.\n\nr0:"
+            " pointer to user\nr1: pointer to target\nr2: bool play animation\nr3: bool"
+            " log failure message\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    TransferNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Transfers all negative status conditions the user has and gives then to"
+            " the target.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     EndSleepClassStatus = Symbol(
         None,
         None,
         None,
         (
             "Cures the target's sleep, sleepless, nightmare, yawn or napping status due"
             " to the action of the user, and prints the event to the log.\n\nr0:"
@@ -18072,14 +18941,25 @@
         (
             "Removes the target's magnet rise status due to the action of the user, and"
             " prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
             " target"
         ),
     )
 
+    TransferNegativeBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to transfer the the negative blinker class status conditions from"
+            " the user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer\nreturn: Whether or not the status could be transferred"
+        ),
+    )
+
     TryTriggerMonsterHouse = Symbol(
         [0x2BDF8],
         [0x2308978],
         None,
         (
             "Triggers a Monster House for an entity, if the right conditions are"
             " met.\n\nConditions: entity is valid and on the team, the tile is a"
@@ -18507,14 +19387,26 @@
         (
             "Inflicts the Sleep status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
             " number of turns\nr3: flag to log a message on failure"
         ),
     )
 
+    IsProtectedFromSleepClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is immune to sleep class status conditions.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nr2: ignore safeguard\nr3:"
+            " ignore other protections (exclusive items + leaf guard)\nstack[0]: flag"
+            " to log a message on failure\nreturn: bool"
+        ),
+    )
+
     TryInflictNightmareStatus = Symbol(
         [0x35B2C],
         [0x23126AC],
         None,
         (
             "Inflicts the Nightmare status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
@@ -19017,91 +19909,638 @@
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
             " to log a message on failure\nr3: flag to only perform the check for"
             " inflicting without actually inflicting\nreturn: Whether or not the status"
             " could be inflicted"
         ),
     )
 
-    TryInflictDestinyBond = Symbol(
+    TryInflictDestinyBondStatus = Symbol(
         [0x39930],
         [0x23164B0],
         None,
         (
             "Inflicts the Destiny Bond status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
-    TryInvisify = Symbol(
+    TryInflictSureShotStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Sure Shot status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWhifferStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Whiffer status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSetDamageStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Set Damage status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictFocusEnergyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Focus Energy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictDecoyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Decoy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictCurseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Curse status condition on a target monster if possible and if"
+            " the user is\na ghost type. Otherwise, just boost the user's defense and"
+            " attack then lower the user's\nspeed.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
+    TryInflictSnatchStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Snatch status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictTauntStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Taunt status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictStockpileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Stockpile condition on a target monster if possible. Won't"
+            " boost the level\nof stockpiling above 3.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nreturn: Whether or not the status could be"
+            " inflicted or boosted"
+        ),
+    )
+
+    TryInflictInvisibleStatus = Symbol(
         [0x3A45C],
         [0x2316FDC],
         None,
         (
             "Attempts to turn the target invisible.\n\nThe user pointer is only used"
             " when calling LogMessage functions.\n\nr0: user entity pointer\nr1: target"
             " entity pointer"
         ),
     )
 
+    TryInflictPerishSongStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Perish Song status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEncoreStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Encore status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryDecreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the belly size of the target. Only when max belly shrink"
+            " is 0, the\ncurrent belly is reduced by belly to lose. If both are"
+            " non-zero, only the max belly\nshrink is applied.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: belly to lose\nr3: max belly"
+            " shrink"
+        ),
+    )
+
+    TryIncreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restore belly and possibly boost max belly of the target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " belly to restore\nr3: max belly boost (if belly is full)\nstack[0]: flag"
+            " to log a message"
+        ),
+    )
+
+    TryInflictMuzzledStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Muzzled status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
     TryTransform = Symbol(
         [0x3B0FC],
         [0x2317C7C],
         None,
         (
             "Attempts to transform the target into the species of a random monster"
             " contained in the list returned by MonsterSpawnListPartialCopy.\n\nThe"
             " user pointer is only used when calling LogMessage functions.\n\nr0: user"
             " entity pointer\nr1: target entity pointer"
         ),
     )
 
+    TryInflictMobileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mobile status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictExposedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Exposed status condition on a target monster if possible."
+            " Only applies to\nGhost types and monsters with raised evasion. If the"
+            " animation effect ID is 0,\ndefaults to animation ID 0xE (this fallback"
+            " animation likely can't be seen in normal\nplay).\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: animation effect ID\nr3: flag to"
+            " only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryActivateIdentifyCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the flag for the identify orb which causes monsters holding items to"
+            " be shown with\na blue exclamation mark status icon.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictBlinkerStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Blinker status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting\nr3:"
+            " flag to log a message on failure\nreturn: Whether or not the status could"
+            " be inflicted"
+        ),
+    )
+
     IsBlinded = Symbol(
         [0x3B6C4],
         [0x2318244],
         None,
         (
             "Returns true if the monster has the blinded status (see"
             " statuses::blinded), or if it is not the leader and is holding Y-Ray"
             " Specs.\n\nr0: pointer to entity\nr1: flag for whether to check for the"
             " held item\nreturn: bool"
         ),
     )
 
+    TryInflictCrossEyedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Cross-Eyed status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEyedropStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Eyedrop status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSlipStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Slip status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nreturn: Whether or not"
+            " the status could be inflicted"
+        ),
+    )
+
+    TryInflictDropeyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Dropeye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
     RestoreMovePP = Symbol(
         [0x3BB00],
         [0x2318680],
         None,
         (
             "Restores the PP of all the target's moves by the specified amount.\n\nr0:"
             " user entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3:"
             " flag to suppress message logging"
         ),
     )
 
-    SetReflectDamageCountdownTo4 = Symbol(
+    ApplyProteinEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: attack boost"
+        ),
+    )
+
+    ApplyCalciumEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's special attack stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special attack boost"
+        ),
+    )
+
+    ApplyIronEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's defense stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: defense boost"
+        ),
+    )
+
+    ApplyZincEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's special defense stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special defense boost"
+        ),
+    )
+
+    TryInflictLongTossStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Long Toss status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictPierceStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Pierce status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictGastroAcidStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Gastro Acid status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    SetAquaRingHealingCountdownTo4 = Symbol(
         [0x3C2A0],
         [0x2318E20],
         None,
         (
-            "Sets the monster's reflect damage countdown to a global value"
+            "Sets the countdown for Aqua Ring healing countdown to a global value"
             " (0x4).\n\nr0: pointer to entity"
         ),
     )
 
+    ApplyAquaRingHealing = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the passive healing gained from the Aqua Ring status.\n\nr0:"
+            " pointer to entity"
+        ),
+    )
+
+    TryInflictAquaRingStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Aqua Ring status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLuckyChantStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Lucky Chant status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictHealBlockStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Heal Block status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    MonsterHasEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the monster has the Embargo status condition.\n\nr0:"
+            " pointer to entity\nreturn: bool"
+        ),
+    )
+
+    LogItemBlockedByEmbargo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Logs the error message when the usage of an item is blocked by"
+            " Embargo.\n\nr0: pointer to entity"
+        ),
+    )
+
+    TryInflictEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Embargo status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictMiracleEyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Miracle Eye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting"
+        ),
+    )
+
+    TryInflictMagnetRiseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magnet Rise status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     HasConditionalGroundImmunity = Symbol(
         [0x3C92C],
         [0x23194AC],
         None,
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    TryInflictSafeguardStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Safeguard status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMistStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mist status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWishStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Wish status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMagicCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magic Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLightScreenStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Light Screen status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictReflectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Reflect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Protect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictEndureStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Endure status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorMoveStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Move status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictConversion2Status = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Conversion2 status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictVitalThrowStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Vital Throw status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryResetStatChanges = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reset the stat changes of the defender.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr3: bool to force animation"
+        ),
+    )
+
     MirrorMoveIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
             " the effects is a status, 2 if it comes from an exclusive item, 0"
@@ -19259,21 +20698,101 @@
         (
             "Seems to apply an item's effect via a giant switch statement?\n\nr3:"
             " attacker pointer\nstack[0]: defender pointer\nstack[1]: thrown item"
             " pointer\nothers: ?"
         ),
     )
 
-    ViolentSeedBoost = Symbol(
+    ApplyCheriBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the paralysis status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyPechaBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the poisoned and badly poisoned status condition. Prints a"
+            " message on\nfailure.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyRawstBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the burn status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyHungerSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Empties the targets belly to cause Hungry Pal status in non-leader"
+            " monsters and\nFamished in the leader monster.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyVileSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Reduces the targets defense and special defense stages to the lowest"
+            " level.\n\nr0: attacker pointer\nr1: defender pointer"
+        ),
+    )
+
+    ApplyViolentSeedEffect = Symbol(
         [0x40D04],
         [0x231D884],
         None,
         (
-            "Applies the Violent Seed boost to an entity.\n\nr0: attacker pointer\nr1:"
-            " defender pointer"
+            "Boosts the target's offensive stats stages to the max.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGinsengEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the power of the move at the top of the target's Move List. Appears"
+            " to have a\nleftover check to boost the power of a move by 3 instead of 1"
+            " that always fails because\nthe chance is 0.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyBlastSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If thrown, unfreeze and deal fixed damage to the defender. If not thrown,"
+            " try to find \na monster in front of the attacker. If a monster is found"
+            " unfreeze and dedal fixed \ndamage to the defender. Appears to have a"
+            " leftover check for if the current fixed room is a boss fight and loads a"
+            " different pointer for the damage when used in a boss room.\nHowever, this"
+            " isn't noticeable because both the normal and boss damage is the"
+            " same.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: bool"
+            " thrown"
         ),
     )
 
     ApplyGummiBoostsDungeonMode = Symbol(
         [0x40FA8],
         [0x231DB28],
         None,
@@ -19315,14 +20834,68 @@
         None,
         (
             "If the target monster is a Linoone, restores all the PP of all the"
             " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
+    ApplyDoughSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a team member, set dough_seed_extra_poke_flag to"
+            " true to \nmake extra poke spawn on the next floor. Otherwise, do"
+            " nothing.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyViaSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to randomly teleport the target with a message for eating the"
+            " seed.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGravelyrockEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restores 10 hunger to the target and will raise the target's IQ if they"
+            " are a bonsly\nor sudowoodo.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyGonePebbleEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Causes a few visual effects, temporarily changes the dungeon music to the"
+            " Goodnight\ntrack, and gives the target the enduring status.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGracideaEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target is Shaymin, attempt to change the target's form to Shaymin"
+            " Sky Forme. Otherwise, do nothing.\n\nr0: user entity pointer\nr1: target"
+            " entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         [0x42878],
         [0x231F3F8],
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -19389,22 +20962,36 @@
         (
             "Blows away the target monster in a given direction if possible.\n\nr0:"
             " user entity pointer\nr1: target entity pointer\nr2: direction ID"
         ),
     )
 
     TryExplosion = Symbol(
-        [0x44670],
-        [0x23211F0],
+        [0x44330],
+        [0x2320EB0],
         None,
         (
             "Creates an explosion if possible.\n\nThe target monster is considered the"
             " source of the explosion.\n\nr0: user entity pointer\nr1: target entity"
             " pointer\nr2: coordinates where the explosion should take place"
-            " (unverified)\nr3: ?\nstack[0]: ?\nstack[1]: damage source (normally"
+            " (center)\nr3: explosion radius (only works correctly with 1 and"
+            " 2)\nstack[0]: damage type\nstack[1]: damage source"
+        ),
+    )
+
+    TryAftermathExplosion = Symbol(
+        [0x44670],
+        [0x23211F0],
+        None,
+        (
+            "Creates the explosion for the ability aftermath if possible.\n\nThe target"
+            " monster is considered the source of the explosion.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: coordinates where the explosion"
+            " should take place (center)\nr3: explosion radius (only works correctly"
+            " with 1 and 2)\nstack[0]: damage type\nstack[1]: damage source (normally"
             " DAMAGE_SOURCE_EXPLOSION)"
         ),
     )
 
     TryWarp = Symbol(
         [0x44BF0],
         [0x2321770],
@@ -19878,14 +21465,57 @@
     GetStairsRoom = Symbol(
         [0x5A478],
         [0x2336FF8],
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    UpdateTrapsVisibility = Symbol(
+        [0x5AF9C],
+        [0x2337B1C],
+        None,
+        (
+            "Exact purpose unknown. Gets called whenever a trap tile is shown or"
+            " hidden.\n\nNo params."
+        ),
+    )
+
+    DrawTileGrid = Symbol(
+        [0x5B478],
+        [0x2337FF8],
+        None,
+        (
+            "Draws a grid on the nearby walkable tiles. Triggered by pressing Y.\n\nr0:"
+            " Coordinates of the entity around which the grid will be drawn\nr1: ?\nr2:"
+            " ?\nr3: ?"
+        ),
+    )
+
+    HideTileGrid = Symbol(
+        [0x5B7EC],
+        [0x233836C],
+        None,
+        (
+            "Hides the grid on the nearby walkable tiles. Triggered by releasing"
+            " Y.\n\nNo params."
+        ),
+    )
+
+    DiscoverMinimap = Symbol(
+        [0x5BA8C],
+        [0x233860C],
+        None,
+        (
+            "Discovers the tiles around the specified position on the minimap.\n\nThe"
+            " discovery radius depends on the visibility range of the floor. If"
+            " display_data::blinded is true, the function returns early without doing"
+            " anything.\n\nr0: Position around which the map should be discovered"
+        ),
+    )
+
     IsWaterTileset = Symbol(
         [0x5BEE4],
         [0x2338A64],
         None,
         (
             "Returns flag tileset_property::is_water_tileset for the current"
             " tileset\n\nreturn: True if the current tileset is a water tileset"
@@ -19954,14 +21584,34 @@
         (
             "Sets the boost_kecleon_shop_spawn_chance field on the dungeon struct"
             " depending on if a team member has the exclusive item effect for more"
             " kecleon shops.\n\nNo params."
         ),
     )
 
+    SetDoughSeedFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the dough_seed_extra_money_flag field on the dungeon struct to the"
+            " given value.\n\nr0: bool to set the flag to"
+        ),
+    )
+
+    TrySpawnDoughSeedPoke = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the dough_seed_extra_money_flag field on the dungeon struct and"
+            " tries to spawn\nextra poke if it is set.\n\nNo params."
+        ),
+    )
+
     IsSecretBazaar = Symbol(
         [0x5C614],
         [0x2339194],
         None,
         "Checks if the current floor is the Secret Bazaar.\n\nreturn: bool",
     )
 
@@ -20012,28 +21662,62 @@
         None,
         (
             "Checks if the current floor is a secret bazaar or a secret"
             " room.\n\nreturn: bool"
         ),
     )
 
+    HiddenStairsPresent = Symbol(
+        [0x5C728],
+        [0x23392A8],
+        None,
+        (
+            "Checks if the hidden stairs are present on this floor.\n\nThe function"
+            " checks that dungeon_generation_info::hidden_stairs_pos isn't (-1,"
+            " -1)\n\nreturn: True if the hidden stairs are present on this floor, false"
+            " otherwise."
+        ),
+    )
+
+    HiddenStairsTrigger = Symbol(
+        [0x5C7E4],
+        [0x2339364],
+        None,
+        (
+            "Called whenever the leader steps on the hidden stairs.\n\nIf the stairs"
+            " hadn't been revealed yet, plays the corresponding animation.\n\nr0: True"
+            " to display a message if the stairs are revealed, false to omit it."
+        ),
+    )
+
     GetDungeonGenInfoUnk0C = Symbol(
         [0x5C8D0], [0x2339450], None, "return: dungeon_generation_info::field_0xc"
     )
 
     GetMinimapData = Symbol(
         [0x5D168],
         [0x2339CE8],
         None,
         (
             "Returns a pointer to the minimap_display_data struct in the dungeon"
             " struct.\n\nreturn: minimap_display_data*"
         ),
     )
 
+    DrawMinimapTile = Symbol(
+        [0x5D23C],
+        [0x2339DBC],
+        None,
+        "Draws a single tile on the minimap.\n\nr0: X position\nr1: Y position",
+    )
+
+    UpdateMinimap = Symbol(
+        [0x5DD38], [0x233A8B8], None, "Graphically updates the minimap\n\nNo params."
+    )
+
     SetMinimapDataE447 = Symbol(
         [0x5E268],
         [0x233ADE8],
         None,
         (
             "Sets minimap_display_data::field_0xE447 to the specified value\n\nr0:"
             " Value to set the field to"
@@ -20057,14 +21741,35 @@
         None,
         (
             "Sets minimap_display_data::field_0xE448 to the specified value\n\nr0:"
             " Value to set the field to"
         ),
     )
 
+    InitWeirdMinimapMatrix = Symbol(
+        [0x5E2F4],
+        [0x233AE74],
+        None,
+        (
+            "Initializes the matrix at minimap_display_data+0xE000. Seems to overflow"
+            " said matrix when doing so.\n\nNo params."
+        ),
+    )
+
+    InitMinimapDisplayTile = Symbol(
+        [0x5E354],
+        [0x233AED4],
+        None,
+        (
+            "Used to initialize an instance of struct minimap_display_tile\n\nr0:"
+            " Pointer to struct to init\nr1: Seems to be a pointer to the file that"
+            " stores minimap icons or something like that"
+        ),
+    )
+
     LoadFixedRoomDataVeneer = Symbol(
         [0x5E688],
         [0x233B208],
         None,
         (
             "Likely a linker-generated veneer for LoadFixedRoomData.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nNo"
@@ -20756,14 +22461,24 @@
             " reached by the traversal algorithm, then the stairs must not be reachable"
             " from that tile.\n\nr0: x coordinate of the stairs\nr1: y coordinate of"
             " the stairs\nr2: flag to always return true, but set a special bit on all"
             " walkable tiles that aren't reachable from the stairs\nreturn: bool"
         ),
     )
 
+    GetNextFixedRoomAction = Symbol(
+        [0x66534],
+        [0x23430B4],
+        None,
+        (
+            "Returns the next action that needs to be performed when spawning a fixed"
+            " room tile.\n\nreturn: Next action ID"
+        ),
+    )
+
     ConvertWallsToChasms = Symbol(
         [0x665AC], [0x234312C], None, "Converts all wall tiles to chasms.\n\nNo params."
     )
 
     ResetInnerBoundaryTileRows = Symbol(
         [0x66BE0],
         [0x2343760],
@@ -20814,25 +22529,75 @@
             " HIDDEN_STAIRS_RANDOM_SECRET_BAZAAR_OR_SECRET_ROOM and the"
             " floor_properties::hidden_stairs_spawn_chance) into a concrete hidden"
             " stairs type.\n\nr0: dungeon generation info pointer\nr1: floor properties"
             " pointer\nreturn: enum hidden_stairs_type"
         ),
     )
 
+    GetFinalKecleonShopSpawnChance = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the kecleon shop spawn chance for the floor.\n\nWhen"
+            " dungeon::boost_kecleon_shop_spawn_chance is false, returns the same value"
+            " as the input. When it's true, returns the input (chance * 1.2).\n\nr0:"
+            " base kecleon shop spawn chance,"
+            " floor_properties::kecleon_shop_spawn_chance\nreturn: int"
+        ),
+    )
+
     ResetHiddenStairsSpawn = Symbol(
         [0x66F6C],
         [0x2343AEC],
         None,
         (
             "Resets hidden stairs spawn information for the floor. This includes the"
             " position on the floor generation status as well as the flag indicating"
             " whether the spawn was blocked.\n\nNo params."
         ),
     )
 
+    PlaceFixedRoomTile = Symbol(
+        [0x66F94],
+        [0x2343B14],
+        None,
+        (
+            "Used to spawn a single tile when generating a fixed room. The tile might"
+            " contain an item or a monster.\n\nr0: Pointer to the tile to spawn\nr1:"
+            " Fixed room action to perform. Controls what exactly will be spawned. The"
+            " action is actually 12 bits long, the highest 4 bits are used as a"
+            " parameter that represents a direction (for example, when spawning a"
+            " monster).\nr2: Tile X position\nr3: Tile Y position"
+        ),
+    )
+
+    FixedRoomActionParamToDirection = Symbol(
+        [0x679D0],
+        [0x2344550],
+        None,
+        (
+            "Converts the parameter stored in a fixed room action value to a direction"
+            " ID.\n\nThe conversion is performed by subtracting 1 to the value. If the"
+            " parameter had a value of 0, DIR_NONE is returned.\n\nr0: Parameter"
+            " value\nreturn: Direction"
+        ),
+    )
+
+    ApplyKeyEffect = Symbol(
+        [0x67D3C],
+        [0x23448BC],
+        None,
+        (
+            "Attempts to open a locked door in front of the target if a locked door has"
+            " not already\nbeen open on the floor.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
     LoadFixedRoomData = Symbol(
         [0x67DF4],
         [0x2344974],
         None,
         (
             "Loads fixed room data from BALANCE/fixed.bin into the buffer pointed to by"
             " FIXED_ROOM_DATA_PTR.\n\nNo params."
@@ -21615,15 +23380,25 @@
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
             " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
-        [0x71E74], [0x234E9F4], None, "Note: unverified, ported from Irdkwia's notes"
+        [0x71E74],
+        [0x234E9F4],
+        None,
+        (
+            "Opens a menu. The menu to open depends on the specified parameter.\n\nIt"
+            " looks like the function takes a parameter in r0, but doesn't use it. r1"
+            " doesn't even get set when this function is called.\n\nr0: (?) Unused by"
+            " the function. Seems to be 1 byte long.\nr1: (?) Unused by the function."
+            " Seems to be 1 byte long.\nr2: True to open the bag menu, false to open"
+            " the main dungeon menu"
+        ),
     )
 
     OthersMenuLoop = Symbol(
         [0x7384C],
         [0x23503CC],
         None,
         (
@@ -21814,27 +23589,30 @@
         0x4,
         (
             "The move target and range code for special healing moves that target just"
             " the user (0x273).\n\ntype: struct move_target_and_range (+ padding)"
         ),
     )
 
-    PLAIN_SEED_VALUE = Symbol(
-        [0x40628], [0x231D1A8], 0x4, "Some value related to the Plain Seed (0xBE9)."
+    PLAIN_SEED_STRING_ID = Symbol(
+        [0x40628], [0x231D1A8], 0x4, "The string ID for eating a Plain Seed (0xBE9)."
     )
 
     MAX_ELIXIR_PP_RESTORATION = Symbol(
         [0x4062C],
         [0x231D1AC],
         0x4,
         "The amount of PP restored per move by ingesting a Max Elixir (0x3E7).",
     )
 
-    SLIP_SEED_VALUE = Symbol(
-        [0x40A94], [0x231D614], 0x4, "Some value related to the Slip Seed (0xC75)."
+    SLIP_SEED_FAIL_STRING_ID = Symbol(
+        [0x40A94],
+        [0x231D614],
+        0x4,
+        "The string ID for when eating the Slip Seed fails (0xC75).",
     )
 
     ROCK_WRECKER_MOVE_ID = Symbol(
         None, None, None, "The move ID for Rock Wrecker (453)."
     )
 
     CASTFORM_NORMAL_FORM_MALE_ID = Symbol(
@@ -22679,15 +24457,28 @@
     loadaddress = 0x233D200
     length = 0xA160
     functions = EuOverlay3Functions
     data = EuOverlay3Data
 
 
 class EuOverlay30Functions:
-    pass
+    WriteQuicksaveData = Symbol(
+        [0x448],
+        [0x2383868],
+        None,
+        (
+            "Function responsible for writing dungeon data when quicksaving.\n\nAmong"
+            " other things, it contains a loop that goes through all the monsters in"
+            " the current dungeon, copying their data to the buffer. The data is not"
+            " copied as-is though, the game uses a reduced version of the monster"
+            " struct containing only the minimum required data to resume the game"
+            " later.\n\nr0: Pointer to buffer where data should be written\nr1: Buffer"
+            " size. Seems to be 0x5800 (22 KB) when the function is called."
+        ),
+    )
 
 
 class EuOverlay30Data:
     OVERLAY30_JP_STRING_1 = Symbol([0x3864], [0x2386C84], 0xC, "みさき様")
 
     OVERLAY30_JP_STRING_2 = Symbol([0x3870], [0x2386C90], 0xC, "やよい様")
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -1020,17 +1020,17 @@
 
     LoadFileInPackWithPackId = Symbol(
         None,
         None,
         None,
         (
             "Call LoadFileInPack after looking up the global Pack archive by its"
-            " identifier\n\nr0: pack file identifier\nr1: [output] target buffer\nr2:"
-            " file index\nreturn: number of read bytes (identical to the length of the"
-            " pack from the Table of Content)"
+            " identifier\n\nr0: pack file identifier\nr1: file index\nr2: [output]"
+            " target buffer\nreturn: number of read bytes (identical to the length of"
+            " the pack from the Table of Content)"
         ),
     )
 
     AllocAndLoadFileInPack = Symbol(
         None,
         None,
         None,
@@ -1071,14 +1071,27 @@
             "Load the indexed file from the Pack archive, itself loaded from the"
             " ROM.\n\nr0: pack file struct\nr1: [output] target buffer\nr2: file"
             " index\nreturn: number of read bytes (identical to the length of the pack"
             " from the Table of Content)"
         ),
     )
 
+    GetDungeonResultMsg = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the message that is shown on the dungeon results ('The Last Outing')"
+            " screen, right after the leader's name.\n\nr0: Damage source value to use"
+            " when displaying the cause of fainting or the result of the"
+            " expedition\nr1: [output] Buffer where the resulting message will be"
+            " stored\nr2: Buffer size\nr3: (?) Seems to point to a buffer"
+        ),
+    )
+
     GetDamageSource = Symbol(
         None,
         None,
         None,
         (
             "Gets the damage source for a given move-item combination.\n\nIf there's no"
             " item, the source is the move ID. If the item is an orb, return"
@@ -1153,14 +1166,26 @@
         None,
         (
             "Checks if an item is one of the aura bows received at the start of the"
             " game.\n\nr0: item ID\nreturn: bool"
         ),
     )
 
+    IsTreasureBox = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the given item ID is a treasure box\n\nIn particular, it checks"
+            " if the category of the item is CATEGORY_TREASURE_BOXES_1,"
+            " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
+            " ID\nreturn: True if the item is a treasure box, false otherwise"
+        ),
+    )
+
     InitItem = Symbol(
         None,
         None,
         None,
         (
             "Initialize an item struct with the given information.\n\nThis will resolve"
             " the quantity based on the item type. For Poké, the quantity code will"
@@ -1441,22 +1466,21 @@
     GetItemMoveId = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: move ID",
     )
 
-    TestItemFlag0xE = Symbol(
+    TestItemAiFlag = Symbol(
         None,
         None,
         None,
         (
-            "Tests bit 7 if r1 is 0, bit 6 if r1 is 1, bit 5 otherwise\n\nNote:"
-            " unverified, ported from Irdkwia's notes\n\nr0: item ID\nr1:"
-            " bit_id\nreturn: bool"
+            "Used to check the AI flags for an item. Tests bit 7 if r1 is 0, bit 6 if"
+            " r1 is 1, bit\n5 otherwise.\n\nr0: item ID\nr1: bit_id\nreturn: bool"
         ),
     )
 
     IsItemInTimeDarkness = Symbol(
         None,
         None,
         None,
@@ -1494,14 +1518,25 @@
         None,
         (
             "Sets the amount of money the player is carrying, clamping the value to the"
             " range [0, MAX_MONEY_CARRIED].\n\nr0: new value"
         ),
     )
 
+    AddMoneyCarried = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds the amount of money to the player's current amount of money. Just"
+            " calls\nSetMoneyCarried with the current money + money gained.\n\nr0:"
+            " money gained (can be negative)"
+        ),
+    )
+
     GetCurrentBagCapacity = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: bag capacity",
     )
 
@@ -1522,15 +1557,18 @@
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: # items",
     )
 
     CountNbItemsOfTypeInBag = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: count",
+        (
+            "Returns the number of items of the given kind in the bag\n\nr0: item"
+            " ID\nreturn: count"
+        ),
     )
 
     CountItemTypeInBag = Symbol(
         None,
         None,
         None,
         (
@@ -1742,14 +1780,24 @@
     ScriptSpecialProcess0x39 = Symbol(
         None,
         None,
         None,
         "Implements SPECIAL_PROC_0x39 (see ScriptSpecialProcessCall).\n\nreturn: bool",
     )
 
+    CountNbItemsOfTypeInStorage = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the number of items of the given kind in the storage\n\nr0: item"
+            " ID\nreturn: count"
+        ),
+    )
+
     CountItemTypeInStorage = Symbol(
         None,
         None,
         None,
         (
             "Implements SPECIAL_PROC_COUNT_ITEM_TYPE_IN_STORAGE (see"
             " ScriptSpecialProcessCall).\n\nr0: pointer to an owned_item\nreturn:"
@@ -2588,38 +2636,62 @@
     StopSe = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
 
     DeleteWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
+            "Always delete an entry if the file is allocated externally"
+            " (file_externally_allocated is set), otherwise, decrease the reference"
+            " counter. If it reach 0, delete the sprite.\n\nr0: wan_table_ptr\nr1:"
             " wan_id"
         ),
     )
 
+    AllocateWanTableEntry = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return the identifier to a free wan table entry (-1 if none are"
+            " avalaible). The entry is zeroed.\n\nr0: wan_table_ptr\nreturn: the entry"
+            " id in wan_table"
+        ),
+    )
+
     FindWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Appears to search in the given table (in practice always seems to be"
+            "Search in the given table (in practice always seems to be"
             " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
             " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
             " if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "wan_id = -1 if it is not loaded\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: wan_table_ptr\nr1: bin_file_id\nr2: file_id\nreturn: wan_id"
+            "Look up a sprite with the provided pack_id and file_index in the wan"
+            " table.\n\nr0: wan_table_ptr\nr1: pack_id\nr2: file_index\nreturn: sprite"
+            " id in the wan table, -1 if not found"
+        ),
+    )
+
+    InitWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the input WAN table with 0x60 free entries (it needs a length"
+            " of 0x1510 bytes)\n\nr0: wan_table_ptr"
         ),
     )
 
     LoadWanTableEntry = Symbol(
         None,
         None,
         None,
@@ -2627,14 +2699,40 @@
             "Appears to load data from the given file (in practice always seems to be"
             " animation data), using previously loaded data in the given table (see"
             " FindWanTableEntry) if possible.\n\nr0: table pointer\nr1: file name\nr2:"
             " flags\nreturn: table index of the loaded data"
         ),
     )
 
+    LoadWanTableEntryFromPack = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3: allocation"
+            " flags\nstack[0]: compressed\nreturn: the entry id in wan_table"
+        ),
+    )
+
+    LoadWanTableEntryFromPackUseProvidedMemory = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite into the"
+            " provided memory area. Mark the sprite as externally allocated.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3:"
+            " sprite_storage_ptr\nstack[0]: compressed\nreturn: the entry id in"
+            " wan_table"
+        ),
+    )
+
     ReplaceWanFromBinFile = Symbol(
         None,
         None,
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
             " wan_id\nr2: bin_file_id\nr3: file_id\nstack[0]: compressed"
@@ -2890,14 +2988,30 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetStringPower = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    GetDungeonResultString = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns a string containing some information to be used when displaying"
+            " the dungeon results screen.\n\nThe exact string returned depends on the"
+            " value of r0:\n0: Name of the move that fainted the leader. Empty string"
+            " if the leader didn't faint.\n1-3: Seems to always result in an empty"
+            " string.\n4: Name of the pokémon that fainted the leader, or name of the"
+            " leader if the leader didn't faint.\n5: Name of the fainted leader. Empty"
+            " string if the leader didn't faint.\n\nr0: String to return\nreturn:"
+            " Pointer to resulting string"
+        ),
+    )
+
     SetQuestionMarks = Symbol(
         None,
         None,
         None,
         (
             "Fills the buffer with the string '???'\n\nNote: unverified, ported from"
             " Irdkwia's notes\n\nr0: buffer"
@@ -3196,15 +3310,15 @@
 
     IsMenuOptionActive = Symbol(
         None,
         None,
         None,
         (
             "Called whenever a menu option is selected. Returns whether the option is"
-            " active or not.\n\nr0: ?\nReturn: True if the menu option is enabled,"
+            " active or not.\n\nr0: ?\nreturn: True if the menu option is enabled,"
             " false otherwise."
         ),
     )
 
     ShowKeyboard = Symbol(
         None,
         None,
@@ -3570,14 +3684,24 @@
         None,
         (
             "Gets the special episode type from the SPECIAL_EPISODE_TYPE script"
             " variable.\n\nreturn: special episode type"
         ),
     )
 
+    GetExecuteSpecialEpisodeType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the special episode type from the EXECUTE_SPECIAL_EPISODE_TYPE script"
+            " variable.\n\nreturn: special episode type"
+        ),
+    )
+
     HasPlayedOldGame = Symbol(
         None,
         None,
         None,
         "Returns the value of the VAR_PLAY_OLD_GAME script variable.\n\nreturn: bool",
     )
 
@@ -3640,21 +3764,21 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: dungeon ID\nr1:"
             " bit_value"
         ),
     )
 
-    CheckDungeonOpen = Symbol(
+    GetDungeonMode = Symbol(
         None,
         None,
         None,
         (
-            "Related to dungeon open list\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: dungeon ID\nreturn: status code?"
+            "Returns the mode of the specified dungeon\n\nr0: Dungeon ID\nreturn:"
+            " Dungeon mode"
         ),
     )
 
     GlobalProgressAlloc = Symbol(
         None,
         None,
         None,
@@ -3861,14 +3985,59 @@
         (
             "If buffer_portrait is null, it only checks if it exists\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: portrait box pointer\nr1:"
             " buffer_portrait\nreturn: exists"
         ),
     )
 
+    SetEnterDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to set the dungeon that will be accessed when switching from ground"
+            " to dungeon mode.\n\nr0: Dungeon ID"
+        ),
+    )
+
+    InitDungeonInit = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the dungeon_init struct before entering a dungeon.\n\nr0:"
+            " [output] Pointer to the struct to init\nr1: Dungeon ID"
+        ),
+    )
+
+    IsNoLossPenaltyDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the specified dungeon shouldn't have a loss penalty.\n\nIf"
+            " true you won't lose your money and items upon fainting. Also used to"
+            " initialize dungeon_init::skip_faint_animation_flag.\n\nReturns: True for"
+            " DUNGEON_CRYSTAL_LAKE and DUNGEON_5TH_STATION_CLEARING, as well as for"
+            " DUNGEON_DEEP_STAR_CAVE_TEAM_ROGUE if the ground variable SIDE01_BOSS2ND"
+            " is 0; false otherwise."
+        ),
+    )
+
+    CheckMissionRestrictions = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Seems to be used to check if you have any missions that have unmet"
+            " restrictions when trying to access a dungeon.\n\nr0: ?\nreturn: (?) Seems"
+            " to be composed of multiple bitflags."
+        ),
+    )
+
     GetNbFloors = Symbol(
         None,
         None,
         None,
         (
             "Returns the number of floors of the given dungeon.\n\nThe result is"
             " hardcoded for certain dungeons, such as dojo mazes.\n\nr0: Dungeon"
@@ -3930,19 +4099,75 @@
         (
             "Given a dungeon ID and a floor number, returns a struct with the"
             " corresponding dungeon group and floor number in that group.\n\nThe"
             " function normally uses the data in mappa_s.bin to calculate the result,"
             " but there's some dungeons (such as dojo mazes) that have hardcoded return"
             " values.\n\nIrdkwia's notes:\n  [r1]: dungeon_id\n  [r1+1]:"
             " dungeon_floor_id\n  [r0]: group_id\n  [r0+1]: group_floor_id\n\nr0:"
-            " (output) Struct containing the dungeon group and floor group\nr1: Struct"
+            " [output] Struct containing the dungeon group and floor group\nr1: Struct"
             " containing the dungeon ID and floor number"
         ),
     )
 
+    GetMissionRank = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the mission rank for the given dungeon and floor.\n\nIf the dungeon"
+            " ID is >= DUNGEON_NORMAL_FLY_MAZE or the group of the dungeon is >"
+            " DGROUP_DUMMY_0x63, returns MISSION_RANK_E.\n\nr0: Dungeon and"
+            " floor\nreturn: Mission rank"
+        ),
+    )
+
+    GetOutlawLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for outlaws for the given dungeon and"
+            " floor\n\nr0: Dungeon and floor\nreturn: Outlaw level"
+        ),
+    )
+
+    GetOutlawLeaderLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for team leader outlaws for the given"
+            " dungeon and floor. Identical to GetOutlawLevel.\n\nr0: Dungeon and"
+            " floor\nreturn: Outlaw leader level"
+        ),
+    )
+
+    GetOutlawMinionLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for minion outlaws for the given"
+            " dungeon and floor.\n\nr0: Dungeon and floor\nreturn: Outlaw minion level"
+        ),
+    )
+
+    AddGuestMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds a guest monster to the active team\n\nr0: dungeon_init struct for the"
+            " dungeon that is about to be entered\nr1: Number of the guest monster to"
+            " add. Used when more than one monster is added.\nr2: Pointer to the guest"
+            " monster entry to add to the team (usually located within"
+            " GUEST_MONSTER_DATA)"
+        ),
+    )
+
     GetGroundNameId = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetAdventureLogStructLocation = Symbol(
         None,
         None,
@@ -5010,14 +5235,24 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: family index",
     )
 
     LoadM2nAndN2m = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    GuestMonsterToGroundMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inits a ground_monster entry with the given guest_monster struct.\n\nr0:"
+            " [output] ground_monster struct to init\nr1: guest_monster struct to use"
+        ),
+    )
+
     StrcmpMonsterName = Symbol(
         None,
         None,
         None,
         (
             "Checks if the string_buffer matches the name of the species\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: string_buffer\nr1: monster"
@@ -5586,15 +5821,15 @@
         None,
         None,
         None,
         (
             "Determines the list of IQ skills that a given monster can learn given its"
             " IQ value.\n\nThe list of skills is written in the array specified in r0."
             " The array has 69 slots in total. Unused slots are set to 0.\n\nr0:"
-            " (output) Array where the list of skills will be written\nr1: Monster"
+            " [output] Array where the list of skills will be written\nr1: Monster"
             " species\nr2: Monster IQ\nreturn: Amount of skills written to the output"
             " array"
         ),
     )
 
     DisableIqSkill = Symbol(
         None,
@@ -6023,26 +6258,121 @@
         (
             "Converts an index in DUNGEON_SWAP_ID_TABLE to the corresponding dungeon"
             " ID, or DUNGEON_DUMMY_0xFF if the index is -1.\n\nr0: index\nreturn:"
             " dungeon ID"
         ),
     )
 
+    GetDungeonModeSpecial = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the status of the given dungeon, with some modifications.\n\nIf"
+            " the dungeon ID is DUNGEON_BEACH, returns DMODE_REQUEST.\nIf it's"
+            " DUNGEON_JOINED_AT_UNKNOWN, returns DMODE_OPEN_AND_REQUEST.\nIf it's >="
+            " DUNGEON_NORMAL_FLY_MAZE and <= DUNGEON_DOJO_0xD3, returns"
+            " DMODE_OPEN_AND_REQUEST.\nElse, calls GetDungeonMode and returns"
+            " DMODE_REQUEST if the dungeon has been cleared, or DMODE_OPEN if it's"
+            " not.\n\nr0: Dungeon ID\nreturn: Dungeon mode"
+        ),
+    )
+
     ResumeBgm = Symbol(
         None, None, None, "Uncertain.\n\nNote: unverified, ported from Irdkwia's notes"
     )
 
     FlushChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     UpdateChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    ClearIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enables processor interrupts by clearing the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were disabled, 0x0 if they were already enabled)"
+        ),
+    )
+
+    EnableIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Disables processor interrupts by setting the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were already disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    SetIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the value of the processor's interrupt flag according to the"
+            " specified parameter.\n\nr0: Value to set the flag to (0x80 to set it,"
+            " which disables interrupts; 0x0 to unset it, which enables"
+            " interrupts)\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts were"
+            " disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    EnableIrqFiqFlags = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Disables processor all interrupts (both standard and fast) by setting the"
+            " i and f flags in the program status register (cpsr).\n\nreturn: Old value"
+            " of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    SetIrqFiqFlags = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the value of the processor's interrupt flags (i and f) according to"
+            " the specified parameter.\n\nr0: Value to set the flags to (0xC0 to set"
+            " both flags, 0x80 to set the i flag and clear the f flag, 0x40 to set the"
+            " f flag and clear the i flag and 0x0 to clear both flags)\nreturn: Old"
+            " value of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    GetIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the current value of the processor's interrupt request (i)"
+            " flag\n\nreturn: cpsr & 0x80 (0x80 if interrupts are disabled, 0x0 if they"
+            " are enabled)"
+        ),
+    )
+
+    WaitForever2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EnableIrqFlag and WaitForInterrupt in an infinite loop.\n\nThis is"
+            " called on fatal errors to hang the program indefinitely.\n\nNo params."
+        ),
+    )
+
     WaitForInterrupt = Symbol(
         None,
         None,
         None,
         (
             "Presumably blocks until the program receives an interrupt.\n\nThis just"
             " calls (in Ghidra terminology) coproc_moveto_Wait_for_interrupt(0). See"
@@ -12617,14 +12947,24 @@
         None,
         (
             "The multiplier for damage from the Air Blade (1.5), as a binary"
             " fixed-point number (8 fraction bits)"
         ),
     )
 
+    KECLEON_SHOP_BOOST_CHANCE_MULTIPLIER = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The boosted kecleon shop spawn chance multiplier (~1.2) as a binary"
+            " fixed-point number (8 fraction bits)."
+        ),
+    )
+
     HIDDEN_STAIRS_SPAWN_CHANCE_MULTIPLIER = Symbol(
         None,
         None,
         None,
         (
             "The hidden stairs spawn chance multiplier (~1.2) as a binary fixed-point"
             " number (8 fraction bits), if applicable. See"
@@ -13301,16 +13641,18 @@
     )
 
     LoadBackgroundAttributes = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: [output]"
-            " bg_attr_str\nr1: bg_id"
+            "Open and read an entry from the MAP_BG/bg_list.dat\n\nDocumentation on"
+            " this format can be found"
+            " here:\nhttps://github.com/SkyTemple/skytemple-files/tree/55b3017631a8a1b0f106111ef91a901dc394c6df/skytemple_files/graphics/bg_list_dat\n\nr0:"
+            " [output] The entry\nr1: background ID"
         ),
     )
 
     LoadMapType10 = Symbol(
         None,
         None,
         None,
@@ -13413,14 +13755,24 @@
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
             " characters printed, excluding the null-terminator"
         ),
     )
 
+    GetExclusiveItemRequirements = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to calculate the items required to get a certain exclusive item in"
+            " the swap shop.\n\nr0: ?\nr1: ?"
+        ),
+    )
+
     StatusUpdate = Symbol(
         None,
         None,
         None,
         (
             "Implements SPECIAL_PROC_STATUS_UPDATE (see"
             " ScriptSpecialProcessCall).\n\nNo params."
@@ -13579,14 +13931,18 @@
         ),
     )
 
     UNIONALL_RAM_ADDRESS = Symbol(None, None, None, "[Runtime]")
 
     GROUND_STATE_MAP = Symbol(None, None, None, "[Runtime]")
 
+    GROUND_STATE_WEATHER = Symbol(
+        None, None, None, "[Runtime] Same structure format as GROUND_STATE_MAP"
+    )
+
     GROUND_STATE_PTRS = Symbol(
         None,
         None,
         None,
         (
             "Host pointers to multiple structure used for performing an overworld"
             " scene\n\ntype: struct main_ground_data"
@@ -15430,24 +15786,81 @@
     FadeToBlack = Symbol(
         None,
         None,
         None,
         "Fades the screen to black across several frames.\n\nNo params.",
     )
 
+    CheckTouchscreenArea = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the currently pressed touchscreen position is within the"
+            " specified area.\n\nr0: Area lower X coordinate\nr1: Area lower Y"
+            " coordinate\nr2: Area upper X coordinate\nr3: Area upper Y"
+            " coordinate\nreturn: True if the specified area contains the currently"
+            " pressed touchscreen position, false otherwise."
+        ),
+    )
+
+    GetTrapInfo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Given a trap entity, returns the pointer to the trap info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Trap data pointer"
+        ),
+    )
+
+    GetItemInfo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Given an item entity, returns the pointer to the item info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Item data pointer"
+        ),
+    )
+
     GetTileAtEntity = Symbol(
         None,
         None,
         None,
         (
             "Returns a pointer to the tile where an entity is located.\n\nr0: pointer"
             " to entity\nreturns: pointer to tile"
         ),
     )
 
+    UpdateEntityPixelPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Updates an entity's pixel_pos field using the specified pixel_position"
+            " struct, or its own pos field if it's null.\n\nr0: Entity pointer\nr1:"
+            " Pixel position to use, or null to use the entity's own position"
+        ),
+    )
+
+    CreateEnemyEntity = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Creates and initializes the entity struct of a newly spawned enemy"
+            " monster. Fails if there's 16 enemies on the floor already.\n\nIt could"
+            " also be used to spawn fixed room allies, since those share their slots on"
+            " the entity list.\n\nr0: Monster ID\nreturn: Pointer to the newly"
+            " initialized entity, or null if the entity couldn't be initialized"
+        ),
+    )
+
     SpawnTrap = Symbol(
         None,
         None,
         None,
         (
             "Spawns a trap on the floor. Fails if there are more than 64 traps already"
             " on the floor.\n\nThis modifies the appropriate fields on the dungeon"
@@ -15467,35 +15880,46 @@
             " items already on the floor.\n\nThis initializes a new entry in the entity"
             " table and points it to the corresponding slot in the item info"
             " list.\n\nr0: position\nreturn: entity pointer for the newly added item,"
             " or null on failure"
         ),
     )
 
-    ShouldDisplayEntityMessages = Symbol(
+    ShouldMinimapDisplayEntity = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if a given entity should be displayed on the minimap\n\nr0: Entity"
+            " pointer\nreturn: True if the entity should be displayed on the minimap"
+        ),
+    )
+
+    ShouldDisplayEntity = Symbol(
         None,
         None,
         None,
         (
-            "Checks if messages that involve a certain entity should be displayed or"
-            " suppressed.\n\nFor example, it returns false if the entity is an"
-            " invisible enemy.\n\nr0: Entity pointer\nr1: ?\nreturn: True if messages"
-            " involving the entity should be displayed, false if they should be"
-            " suppressed."
+            "Checks if an entity should be displayed or not.\n\nFor example, it returns"
+            " false if the entity is an invisible enemy.\nAlso used to determine if"
+            " messages that involve a certain entity should be displayed or"
+            " suppressed.\n\nr0: Entity pointer\nr1: (?) Seems to be 1 for monsters and"
+            " 0 for items.\nreturn: True if the entity and its associated messages"
+            " should be displayed, false if they shouldn't."
         ),
     )
 
-    ShouldDisplayEntityMessagesWrapper = Symbol(
+    ShouldDisplayEntityWrapper = Symbol(
         None,
         None,
         None,
         (
-            "Calls ShouldDisplayEntityMessages with r1 = 0\n\nr0: Entity"
-            " pointer\nreturn: True if messages involving the entity should be"
-            " displayed, false if they should be suppressed."
+            "Calls ShouldDisplayEntity with r1 = 0\n\nr0: Entity pointer\nreturn: True"
+            " if the entity and its associated messages should be displayed, false if"
+            " they shouldn't."
         ),
     )
 
     CanSeeTarget = Symbol(
         None,
         None,
         None,
@@ -15615,28 +16039,54 @@
         (
             "Returns dungeon::display_data::visibility_range. If the visibility range"
             " is 0, returns 2 instead.\n\nreturn: Visibility range of the current"
             " floor, or 2 if the visibility is 0."
         ),
     )
 
-    PlayEffectAnimation = Symbol(
+    PlayEffectAnimationEntity = Symbol(
         None,
         None,
         None,
         (
             "Just a guess. This appears to be paired often with"
             " GetEffectAnimationField0x19, and also has calls AnimationHasMoreFrames in"
             " a loop alongside AdvanceFrame(66) calls.\n\nThe third parameter skips the"
             " loop entirely. It seems like in this case the function might just preload"
-            " some animation frames for later use??\n\nr0: entity pointer\nr1: ?\nr2:"
-            " appears to be a flag for actually running the animation now? If this is"
-            " 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn: status"
-            " code, or maybe the number of frames or something? Either way, -1 seems to"
-            " indicate the animation being finished or something?"
+            " some animation frames for later use??\n\nr0: entity pointer\nr1: Effect"
+            " ID\nr2: appears to be a flag for actually running the animation now? If"
+            " this is 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn:"
+            " status code, or maybe the number of frames or something? Either way, -1"
+            " seems to indicate the animation being finished or something?"
+        ),
+    )
+
+    PlayEffectAnimationPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Takes a position struct in r0 and converts it to a pixel position struct"
+            " before calling PlayEffectAnimationPixelPos\n\nr0: Position where the"
+            " effect should be played\nr1: Effect ID\nr2: Unknown flag (same as the one"
+            " in PlayEffectAnimationEntity)\nreturn: Result of call to"
+            " PlayEffectAnimationPixelPos"
+        ),
+    )
+
+    PlayEffectAnimationPixelPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Seems like a variant of PlayEffectAnimationEntity that uses pixel"
+            " coordinates as its first parameter instead of an entity pointer.\n\nr0:"
+            " Pixel position where the effect should be played\nr1: Effect ID\nr2:"
+            " Unknown flag (same as the one in PlayEffectAnimationEntity)\nreturn: Same"
+            " as PlayEffectAnimationEntity"
         ),
     )
 
     UpdateStatusIconFlags = Symbol(
         None,
         None,
         None,
@@ -15724,15 +16174,15 @@
         None,
         None,
         (
             "Copies all entries in the floor's monster spawn list that have a sprite"
             " size >= 6 to the specified buffer.\n\nThe parameter in r1 can be used to"
             " specify how many entries are already present in the buffer. Entries added"
             " by this function will be placed after those, and the total returned in r1"
-            " will account for existing entries as well.\n\nr0: (output) Buffer where"
+            " will account for existing entries as well.\n\nr0: [output] Buffer where"
             " the result will be stored\nr1: Current amount of entries in the"
             " buffer\nreturn: New amount of entries in the buffer"
         ),
     )
 
     IsOnMonsterSpawnList = Symbol(
         None,
@@ -16104,14 +16554,26 @@
             " the effect of the Switcher Orb). \n\nThe function checks for the Suction"
             " Cups ability for both the user and the target, and for the Mold Breaker"
             " ability on the user.\n\nr0: pointer to user entity\nr1: pointer to target"
             " entity"
         ),
     )
 
+    SetLeaderActionFields = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the leader's monster::action::action_id to the specified"
+            " value.\n\nAlso sets monster::action::action_use_idx and"
+            " monster::action::field_0xA to 0, as well as monster::action::field_0x10"
+            " and monster::action::field_0x12 to -1.\n\nr0: ID of the action to set"
+        ),
+    )
+
     ClearMonsterActionFields = Symbol(
         None,
         None,
         None,
         (
             "Clears the fields related to AI in the monster's data struct, setting them"
             " all to 0.\nSpecifically, monster::action::action_id,"
@@ -16191,14 +16653,27 @@
         (
             "Sets a monster's action to action::ACTION_REGULAR_ATTACK, with a specified"
             " direction.\n\nr0: Pointer to the monster's action field\nr1: Direction in"
             " which to use the move. Gets stored in monster::action::direction."
         ),
     )
 
+    SetActionUseMovePlayer = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets a monster's action to action::ACTION_USE_MOVE_PLAYER, with a"
+            " specified monster and move index.\n\nr0: Pointer to the monster's action"
+            " field\nr1: Index of the monster that is using the move on the entity"
+            " list. Gets stored in monster::action::action_use_idx.\nr2: Index of the"
+            " move to use (0-3). Gets stored in monster::action::field_0xA."
+        ),
+    )
+
     SetActionUseMoveAi = Symbol(
         None,
         None,
         None,
         (
             "Sets a monster's action to action::ACTION_USE_MOVE_AI, with a specified"
             " direction and move index.\n\nr0: Pointer to the monster's action"
@@ -16345,14 +16820,169 @@
             "If the flag for a trapper trap is set, handles spawning a trap based upon"
             " the\ninformation inside the dungeon struct. Uses the entity for logging a"
             " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
             " true if a trap was spawned succesfully"
         ),
     )
 
+    TryTriggerTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called whenever a monster steps on a trap.\n\nThe function will try to"
+            " trigger it. Nothing will happen if the pokémon has the same team as the"
+            " trap. The attempt to trigger the trap can also fail due to IQ skills, due"
+            " to the trap failing to work (random chance), etc.\n\nr0: Entity who"
+            " stepped on the trap\nr1: Trap position\nr2: ?\nr3: ?"
+        ),
+    )
+
+    ApplyMudTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly lowers attack, special attack, defense, or special defense of the"
+            " defender by 3 stages.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer"
+        ),
+    )
+
+    ApplyStickyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to make something in the bag"
+            " sticky. Otherwise, try to make the item the monster is holding"
+            " sticky.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyGrimyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to turn food items in the"
+            " toolbox into\ngrimy food. Otherwise, try to make the food item the"
+            " monster is holding grimy food.\n\nr0: attacker entity pointer\nr1:"
+            " defender entity pointer"
+        ),
+    )
+
+    ApplyPitfallTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, end the current floor unless it has a"
+            " rescue point.\nOtherwise, make the entity faint and ignore reviver seeds."
+            " If not called by a random\ntrap, break the grate on the pitfall"
+            " trap.\n\nr0: attacker entity pointer\nr1: defender entity pointer\nr2:"
+            " tile pointer\nr3: bool caused by random trap"
+        ),
+    )
+
+    ApplySummonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly spawns 2-4 enemy monsters around the position. The entity is only"
+            " used for\nlogging messages.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyPpZeroTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the PP of one of the defender's moves to 0.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyPokemonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Turns item in the same room as the tile at the position (usually just the"
+            " entities's\nposition) into monsters. If the position is in a hallway,"
+            " convert items in a 3x3 area\ncentered on the position into"
+            " monsters.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTripTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to drop the defender's item and places it on the floor.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyToxicSpikesTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to inflict 10 damage on the defender and then tries to poison"
+            " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyRandomTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Selects a random trap that isn't a wonder tile and isn't a random trap and"
+            " calls\nApplyTrapEffect on all monsters that is different from the trap's"
+            " team.\n\nr0: Triggered trap\nr1: User\nr2: Target, normally same as"
+            " user\nr3: Tile that contains the trap\nstack[0]: position"
+        ),
+    )
+
+    ApplyGrudgeTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Spawns several monsters around the position and gives all monsters on the"
+            " floor the\ngrudge status condition.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Performs the effect of a triggered trap.\n\nThe trap's animation happens"
+            " before this function is called.\n\nr0: Triggered trap\nr1: User\nr2:"
+            " Target, normally same as user\nr3: Tile that contains the trap\nstack[0]:"
+            " position\nstack[1]: trap ID\nstack[2]: bool caused by random"
+            " trap\nreturn: True if the trap should be destroyed after the effect is"
+            " applied"
+        ),
+    )
+
+    RevealTrapsNearby = Symbol(
+        None,
+        None,
+        None,
+        "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16376,28 +17006,63 @@
         None,
         (
             "Returns a pointer to the action data of the current leader (field 0x4A on"
             " its monster struct).\n\nNo params."
         ),
     )
 
+    GetEntityTouchscreenArea = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the area on the touchscreen that contains the sprite of the"
+            " specified entity\n\nr0: Entity pointer\nr1: [output] struct where the"
+            " result should be written"
+        ),
+    )
+
     SetLeaderAction = Symbol(
         None,
         None,
         None,
         (
             "Sets the leader's action field depending on the inputs given by the"
             " player.\n\nThis function also accounts for other special situations that"
             " can force a certain action, such as when the leader is running. The"
             " function also takes care of opening the main menu when X is pressed.\nThe"
             " function generally doesn't return until the player has an action"
             " set.\n\nNo params."
         ),
     )
 
+    ShouldLeaderKeepRunning = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Determines if the leader should keep running. Returns false if the leader"
+            " bumps into something, or if an action that should stop the leader takes"
+            " place.\n\nreturn: True if the leader should keep running, false if it"
+            " should stop."
+        ),
+    )
+
+    CheckLeaderTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the tile the leader just stepped on and performs any required"
+            " actions, such as picking up items, triggering traps, etc.\n\nContains a"
+            " switch that checks the type of the tile the leader just stepped on.\n\nNo"
+            " params."
+        ),
+    )
+
     ChangeLeader = Symbol(
         None,
         None,
         None,
         (
             "Tries to change the current leader to the monster specified by"
             " dungeon::new_leader.\n\nAccounts for situations that can prevent changing"
@@ -16537,14 +17202,25 @@
         (
             "Handles a fainted pokémon (reviving does not count as fainting).\n\nr0:"
             " Fainted entity\nr1: Damage source (move ID or greater than the max move"
             " id for other causes)\nr2: Entity responsible of the fainting"
         ),
     )
 
+    MoveMonsterToPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Moves a monster to the target position. Used both for regular movement and"
+            " special movement (like teleportation).\n\nr0: Entity pointer\nr1: X"
+            " target position\nr2: Y target position\nr3: ?"
+        ),
+    )
+
     UpdateAiTargetPos = Symbol(
         None,
         None,
         None,
         (
             "Given a monster, updates its target_pos field based on its current"
             " position and the direction in which it plans to attack.\n\nr0: Entity"
@@ -16669,14 +17345,24 @@
             "Restores PP for all moves, clears flags move::f_consume_2_pp,"
             " move::flags2_unk5 and move::flags2_unk7, and sets flag"
             " move::f_consume_pp.\nCalled when a monster is revived.\n\nr0: pointer to"
             " entity whose moves will be restored"
         ),
     )
 
+    BoostIQ = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's IQ.\n\nr0: monster entity pointer\nr1: iq"
+            " boost\nr2: bool suppress logs"
+        ),
+    )
+
     ShouldMonsterHeadToStairs = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given monster should try to reach the stairs when controlled"
             " by the AI\n\nr0: Entity pointer\nreturn: True if the monster should try"
@@ -16693,14 +17379,28 @@
             " dungeon::mew_cannot_spawn or the second parameter are true.\n\nCalled"
             " before spawning an enemy, appears to be checking if Mew can spawn on the"
             " current floor.\n\nr0: monster id\nr1: return false if the monster id is"
             " Mew\nreturn: bool"
         ),
     )
 
+    TryEndStatusWithAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if any of the defender's active abilities would end one of their"
+            " current status\nconditions. For example, if the ability Own Tempo will"
+            " stop confusion.\n\nCalled after changing a monster's ability with skill"
+            " swap, role play, or trace to\nremove statuses the monster should no"
+            " longer be affected by.\n\nr0: attacker entity pointer\nr1: defender"
+            " entity pointer"
+        ),
+    )
+
     ExclusiveItemEffectIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is a team member under the effects of a certain"
             " exclusive item effect.\n\nr0: entity pointer\nr1: exclusive item effect"
@@ -16830,14 +17530,27 @@
             "Checks if a monster does not gain experience.\n\nThis basically just"
             " inverts IsSpecialStoryAlly, with the exception of also checking for the"
             " 'Joined At' field being DUNGEON_CLIENT (is this set for mission"
             " clients?).\n\nr0: monster pointer\nreturn: bool"
         ),
     )
 
+    InitOtherMonsterData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes stats, IQ skills and moves for a given monster\n\nMight only"
+            " be used when spawning fixed room monsters.\n\nr0: Entity pointer\nr1:"
+            " Fixed room monster stats index\nr2: Spawn direction? (when calling this"
+            " function while spawning a fixed room monster, this is the parameter value"
+            " associated to the spawn action, after converting it to a direction.)"
+        ),
+    )
+
     SpawnTeam = Symbol(
         None,
         None,
         None,
         "Seems to initialize and spawn the team when entering a dungeon.\n\nr0: ?",
     )
 
@@ -16881,16 +17594,28 @@
     )
 
     InitMonster = Symbol(
         None,
         None,
         None,
         (
-            "Initializes a monster struct.\n\nr0: pointer to monster to initialize\nr1:"
-            " some flag"
+            "Initializes the monster struct within the provided entity struct.\n\nr0:"
+            " ?\nr1: Pointer to the entity whose monster struct should be"
+            " initialized\nr2: pointer to the entity's spawned_monster_data struct\nr3:"
+            " (?) Pointer to something"
+        ),
+    )
+
+    SubInitMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called by InitMonster. Initializes some fields on the monster"
+            " struct.\n\nr0: pointer to monster to initialize\nr1: some flag"
         ),
     )
 
     MarkShopkeeperSpawn = Symbol(
         None,
         None,
         None,
@@ -16995,14 +17720,24 @@
         (
             "Returns the number of attacks that a monster can do in one turn (1 or"
             " 2).\n\nChecks for the abilities Swift Swim, Chlorophyll, Unburden, and"
             " for exclusive items.\n\nr0: pointer to entity\nreturns: int"
         ),
     )
 
+    GetMonsterDisplayNameType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Determines how the name of a monster should be displayed.\n\nr0: Entity"
+            " pointer\nreturn: Display name type"
+        ),
+    )
+
     GetMonsterName = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: buffer\nr1: TargetInfo",
     )
 
@@ -17153,14 +17888,39 @@
         None,
         (
             "Checks if a monster has the sleep, nightmare, or napping status.\n\nr0:"
             " entity pointer\nreturn: bool"
         ),
     )
 
+    CanMonsterMoveInDirection = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the given monster can move in the specified direction\n\nReturns"
+            " false if any monster is standing on the target tile\n\nr0: Monster entity"
+            " pointer\nr1: Direction to check\nreturn: bool"
+        ),
+    )
+
+    GetFinalMobilityType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the mobility type of a monster, after accounting for things that"
+            " could affect it (like items or IQ skills)\n\nIf the specified direction"
+            " is DIR_NONE, direction checks are skipped. If it's not,"
+            " MOBILITY_INTANGIBLE is only returned if the direction is not"
+            " diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility type\nr2:"
+            " Direction of mobility\nreturn: Final mobility type"
+        ),
+    )
+
     IsMonsterCornered = Symbol(
         None,
         None,
         None,
         (
             "True if the given monster is cornered (it can't move in any"
             " direction)\n\nr0: Entity pointer\nreturn: True if the monster can't move"
@@ -17188,15 +17948,15 @@
         None,
         None,
         (
             "Checks whether an AI-controlled monster can move in the specified"
             " direction.\nAccounts for walls, other monsters on the target position and"
             " IQ skills that might prevent a monster from moving into a specific"
             " location, such as House Avoider, Trap Avoider or Lava Evader.\n\nr0:"
-            " Entity pointer\nr1: Direction\nr2: (output) True if movement was not"
+            " Entity pointer\nr1: Direction\nr2: [output] True if movement was not"
             " possible because there was another monster on the target tile, false"
             " otherwise.\nreturn: True if the monster can move in the specified"
             " direction, false otherwise."
         ),
     )
 
     ShouldMonsterRunAway = Symbol(
@@ -17216,14 +17976,47 @@
         (
             "Calls ShouldMonsterRunAway and returns its result. It also calls another"
             " function if the result was true.\n\nr0: Entity pointer\nr1: ?\nreturn:"
             " Result of the call to ShouldMonsterRunAway"
         ),
     )
 
+    SafeguardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Safeguard.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: flag to log a message\nreturn:"
+            " bool"
+        ),
+    )
+
+    LeafGuardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is protected by the ability Leaf Guard.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer\nr2: flag to log a"
+            " message\nreturn: bool"
+        ),
+    )
+
+    IsProtectedFromStatDrops = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting their stats dropped"
+            " by the user.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     NoGastroAcidStatus = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster does not have the Gastro Acid status.\n\nr0: entity"
             " pointer\nreturn: bool"
@@ -17384,14 +18177,25 @@
             "Updates monster::state_flags and monster::prev_state_flags with new"
             " values.\n\nr0: monster pointer\nr1: bitmask for bits to update\nr2:"
             " whether to set the bits indicated by the mask to 1 or 0\nreturn: whether"
             " or not any of the masked bits changed from the previous state"
         ),
     )
 
+    IsProtectedFromNegativeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting a negative status"
+            " condition.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     AddExpSpecial = Symbol(
         None,
         None,
         None,
         (
             "Adds to a monster's experience points, subject to experience boosting"
             " effects.\n\nThis function appears to be called only under special"
@@ -17405,17 +18209,31 @@
     )
 
     EnemyEvolution = Symbol(
         None,
         None,
         None,
         (
-            "Checks if the specified enemy should evolve because it just defeated an"
-            " ally, and if so, attempts to evolve it.\n\nr0: Pointer to the enemy to"
-            " check"
+            "Checks if any enemies on the floor should evolve and attempts to evolve"
+            " it. The\nentity pointer passed seems to get replaced by a generic"
+            " placeholder entity if the\nentity pointer passed is invalid.\n\nr0:"
+            " entity pointer"
+        ),
+    )
+
+    LevelUpItemEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to level up the the target. Calls LevelUp with a few extra checks"
+            " and messages\nfor using as an item. Used for the Joy Seed and Golden"
+            " Seed.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: number"
+            " of levels\nr3: bool message flag?\nstack[0]: bool show level up dialog"
+            " (for example 'Hey, I leveled up!' with a portrait)?"
         ),
     )
 
     TryDecreaseLevel = Symbol(
         None,
         None,
         None,
@@ -17427,27 +18245,31 @@
     )
 
     LevelUp = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: user entity"
-            " pointer\nr1: target entity pointer\nr2: message flag?\nr3: ?\nreturn:"
-            " success flag?"
+            "Attempts to level up the the target. Fails if the target's level can't be"
+            " raised. The show show level up dialog bool does nothing for monsters not"
+            " on the team.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " bool message flag?\nr3: bool show level up dialog (for example 'Hey, I"
+            " leveled up!' with a portrait)?\nreturn: success flag"
         ),
     )
 
     EvolveMonster = Symbol(
         None,
         None,
         None,
         (
-            "Makes the specified monster evolve into the specified species.\n\nr0:"
-            " Pointer to the entity to evolve\nr1: ?\nr2: Species to evolve into"
+            "Makes the specified monster evolve into the specified species. Has a"
+            " special case when\na monster evolves into Ninjask and tries to spawn a"
+            " Shedinja as well.\n\nr0: user entity pointer?\nr1: target pointer to the"
+            " entity to evolve\nr2: Species to evolve into"
         ),
     )
 
     GetSleepAnimationId = Symbol(
         None,
         None,
         None,
@@ -17469,14 +18291,58 @@
             " example, this delayed display system is used to display multiple monsters"
             " moving at once even though they take turns sequentially.\n\nr0: Pointer"
             " to an entity. Can be null.\nreturns: Seems to be true if there were any"
             " pending actions to display."
         ),
     )
 
+    CheckNonLeaderTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Similar to CheckLeaderTile, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: Entity pointer"
+        ),
+    )
+
+    EndNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Cures the target's negative status conditions. The game rarely (if not"
+            " never) calls\nthis function with the bool to remove the wrapping status"
+            " false.\n\nr0: pointer to user\nr1: pointer to target\nr2: bool play"
+            " animation\nr3: bool log failure message\nstack[0]: bool remove wrapping"
+            " status\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    EndNegativeStatusConditionWrapper = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EndNegativeStatusCondition with remove wrapping status false.\n\nr0:"
+            " pointer to user\nr1: pointer to target\nr2: bool play animation\nr3: bool"
+            " log failure message\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    TransferNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Transfers all negative status conditions the user has and gives then to"
+            " the target.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     EndSleepClassStatus = Symbol(
         None,
         None,
         None,
         (
             "Cures the target's sleep, sleepless, nightmare, yawn or napping status due"
             " to the action of the user, and prints the event to the log.\n\nr0:"
@@ -17582,14 +18448,25 @@
         (
             "Removes the target's magnet rise status due to the action of the user, and"
             " prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
             " target"
         ),
     )
 
+    TransferNegativeBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to transfer the the negative blinker class status conditions from"
+            " the user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer\nreturn: Whether or not the status could be transferred"
+        ),
+    )
+
     TryTriggerMonsterHouse = Symbol(
         None,
         None,
         None,
         (
             "Triggers a Monster House for an entity, if the right conditions are"
             " met.\n\nConditions: entity is valid and on the team, the tile is a"
@@ -18017,14 +18894,26 @@
         (
             "Inflicts the Sleep status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
             " number of turns\nr3: flag to log a message on failure"
         ),
     )
 
+    IsProtectedFromSleepClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is immune to sleep class status conditions.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nr2: ignore safeguard\nr3:"
+            " ignore other protections (exclusive items + leaf guard)\nstack[0]: flag"
+            " to log a message on failure\nreturn: bool"
+        ),
+    )
+
     TryInflictNightmareStatus = Symbol(
         None,
         None,
         None,
         (
             "Inflicts the Nightmare status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
@@ -18527,91 +19416,638 @@
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
             " to log a message on failure\nr3: flag to only perform the check for"
             " inflicting without actually inflicting\nreturn: Whether or not the status"
             " could be inflicted"
         ),
     )
 
-    TryInflictDestinyBond = Symbol(
+    TryInflictDestinyBondStatus = Symbol(
         None,
         None,
         None,
         (
             "Inflicts the Destiny Bond status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
-    TryInvisify = Symbol(
+    TryInflictSureShotStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Sure Shot status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWhifferStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Whiffer status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSetDamageStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Set Damage status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictFocusEnergyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Focus Energy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictDecoyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Decoy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictCurseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Curse status condition on a target monster if possible and if"
+            " the user is\na ghost type. Otherwise, just boost the user's defense and"
+            " attack then lower the user's\nspeed.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
+    TryInflictSnatchStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Snatch status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictTauntStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Taunt status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictStockpileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Stockpile condition on a target monster if possible. Won't"
+            " boost the level\nof stockpiling above 3.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nreturn: Whether or not the status could be"
+            " inflicted or boosted"
+        ),
+    )
+
+    TryInflictInvisibleStatus = Symbol(
         None,
         None,
         None,
         (
             "Attempts to turn the target invisible.\n\nThe user pointer is only used"
             " when calling LogMessage functions.\n\nr0: user entity pointer\nr1: target"
             " entity pointer"
         ),
     )
 
+    TryInflictPerishSongStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Perish Song status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEncoreStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Encore status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryDecreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the belly size of the target. Only when max belly shrink"
+            " is 0, the\ncurrent belly is reduced by belly to lose. If both are"
+            " non-zero, only the max belly\nshrink is applied.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: belly to lose\nr3: max belly"
+            " shrink"
+        ),
+    )
+
+    TryIncreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restore belly and possibly boost max belly of the target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " belly to restore\nr3: max belly boost (if belly is full)\nstack[0]: flag"
+            " to log a message"
+        ),
+    )
+
+    TryInflictMuzzledStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Muzzled status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
     TryTransform = Symbol(
         None,
         None,
         None,
         (
             "Attempts to transform the target into the species of a random monster"
             " contained in the list returned by MonsterSpawnListPartialCopy.\n\nThe"
             " user pointer is only used when calling LogMessage functions.\n\nr0: user"
             " entity pointer\nr1: target entity pointer"
         ),
     )
 
+    TryInflictMobileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mobile status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictExposedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Exposed status condition on a target monster if possible."
+            " Only applies to\nGhost types and monsters with raised evasion. If the"
+            " animation effect ID is 0,\ndefaults to animation ID 0xE (this fallback"
+            " animation likely can't be seen in normal\nplay).\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: animation effect ID\nr3: flag to"
+            " only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryActivateIdentifyCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the flag for the identify orb which causes monsters holding items to"
+            " be shown with\na blue exclamation mark status icon.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictBlinkerStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Blinker status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting\nr3:"
+            " flag to log a message on failure\nreturn: Whether or not the status could"
+            " be inflicted"
+        ),
+    )
+
     IsBlinded = Symbol(
         None,
         None,
         None,
         (
             "Returns true if the monster has the blinded status (see"
             " statuses::blinded), or if it is not the leader and is holding Y-Ray"
             " Specs.\n\nr0: pointer to entity\nr1: flag for whether to check for the"
             " held item\nreturn: bool"
         ),
     )
 
+    TryInflictCrossEyedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Cross-Eyed status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEyedropStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Eyedrop status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSlipStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Slip status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nreturn: Whether or not"
+            " the status could be inflicted"
+        ),
+    )
+
+    TryInflictDropeyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Dropeye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
     RestoreMovePP = Symbol(
         None,
         None,
         None,
         (
             "Restores the PP of all the target's moves by the specified amount.\n\nr0:"
             " user entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3:"
             " flag to suppress message logging"
         ),
     )
 
-    SetReflectDamageCountdownTo4 = Symbol(
+    ApplyProteinEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: attack boost"
+        ),
+    )
+
+    ApplyCalciumEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's special attack stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special attack boost"
+        ),
+    )
+
+    ApplyIronEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's defense stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: defense boost"
+        ),
+    )
+
+    ApplyZincEffect = Symbol(
         None,
         None,
         None,
         (
-            "Sets the monster's reflect damage countdown to a global value"
+            "Tries to boost the target's special defense stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special defense boost"
+        ),
+    )
+
+    TryInflictLongTossStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Long Toss status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictPierceStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Pierce status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictGastroAcidStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Gastro Acid status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    SetAquaRingHealingCountdownTo4 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the countdown for Aqua Ring healing countdown to a global value"
             " (0x4).\n\nr0: pointer to entity"
         ),
     )
 
+    ApplyAquaRingHealing = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the passive healing gained from the Aqua Ring status.\n\nr0:"
+            " pointer to entity"
+        ),
+    )
+
+    TryInflictAquaRingStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Aqua Ring status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLuckyChantStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Lucky Chant status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictHealBlockStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Heal Block status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    MonsterHasEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the monster has the Embargo status condition.\n\nr0:"
+            " pointer to entity\nreturn: bool"
+        ),
+    )
+
+    LogItemBlockedByEmbargo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Logs the error message when the usage of an item is blocked by"
+            " Embargo.\n\nr0: pointer to entity"
+        ),
+    )
+
+    TryInflictEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Embargo status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictMiracleEyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Miracle Eye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting"
+        ),
+    )
+
+    TryInflictMagnetRiseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magnet Rise status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     HasConditionalGroundImmunity = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    TryInflictSafeguardStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Safeguard status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMistStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mist status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWishStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Wish status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMagicCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magic Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLightScreenStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Light Screen status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictReflectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Reflect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Protect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictEndureStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Endure status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorMoveStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Move status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictConversion2Status = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Conversion2 status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictVitalThrowStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Vital Throw status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryResetStatChanges = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reset the stat changes of the defender.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr3: bool to force animation"
+        ),
+    )
+
     MirrorMoveIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
             " the effects is a status, 2 if it comes from an exclusive item, 0"
@@ -18769,21 +20205,101 @@
         (
             "Seems to apply an item's effect via a giant switch statement?\n\nr3:"
             " attacker pointer\nstack[0]: defender pointer\nstack[1]: thrown item"
             " pointer\nothers: ?"
         ),
     )
 
-    ViolentSeedBoost = Symbol(
+    ApplyCheriBerryEffect = Symbol(
         None,
         None,
         None,
         (
-            "Applies the Violent Seed boost to an entity.\n\nr0: attacker pointer\nr1:"
-            " defender pointer"
+            "Tries to heal the paralysis status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyPechaBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the poisoned and badly poisoned status condition. Prints a"
+            " message on\nfailure.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyRawstBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the burn status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyHungerSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Empties the targets belly to cause Hungry Pal status in non-leader"
+            " monsters and\nFamished in the leader monster.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyVileSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Reduces the targets defense and special defense stages to the lowest"
+            " level.\n\nr0: attacker pointer\nr1: defender pointer"
+        ),
+    )
+
+    ApplyViolentSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the target's offensive stats stages to the max.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGinsengEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the power of the move at the top of the target's Move List. Appears"
+            " to have a\nleftover check to boost the power of a move by 3 instead of 1"
+            " that always fails because\nthe chance is 0.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyBlastSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If thrown, unfreeze and deal fixed damage to the defender. If not thrown,"
+            " try to find \na monster in front of the attacker. If a monster is found"
+            " unfreeze and dedal fixed \ndamage to the defender. Appears to have a"
+            " leftover check for if the current fixed room is a boss fight and loads a"
+            " different pointer for the damage when used in a boss room.\nHowever, this"
+            " isn't noticeable because both the normal and boss damage is the"
+            " same.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: bool"
+            " thrown"
         ),
     )
 
     ApplyGummiBoostsDungeonMode = Symbol(
         None,
         None,
         None,
@@ -18825,14 +20341,68 @@
         None,
         (
             "If the target monster is a Linoone, restores all the PP of all the"
             " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
+    ApplyDoughSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a team member, set dough_seed_extra_poke_flag to"
+            " true to \nmake extra poke spawn on the next floor. Otherwise, do"
+            " nothing.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyViaSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to randomly teleport the target with a message for eating the"
+            " seed.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGravelyrockEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restores 10 hunger to the target and will raise the target's IQ if they"
+            " are a bonsly\nor sudowoodo.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyGonePebbleEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Causes a few visual effects, temporarily changes the dungeon music to the"
+            " Goodnight\ntrack, and gives the target the enduring status.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGracideaEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target is Shaymin, attempt to change the target's form to Shaymin"
+            " Sky Forme. Otherwise, do nothing.\n\nr0: user entity pointer\nr1: target"
+            " entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -18906,15 +20476,29 @@
         None,
         None,
         None,
         (
             "Creates an explosion if possible.\n\nThe target monster is considered the"
             " source of the explosion.\n\nr0: user entity pointer\nr1: target entity"
             " pointer\nr2: coordinates where the explosion should take place"
-            " (unverified)\nr3: ?\nstack[0]: ?\nstack[1]: damage source (normally"
+            " (center)\nr3: explosion radius (only works correctly with 1 and"
+            " 2)\nstack[0]: damage type\nstack[1]: damage source"
+        ),
+    )
+
+    TryAftermathExplosion = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Creates the explosion for the ability aftermath if possible.\n\nThe target"
+            " monster is considered the source of the explosion.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: coordinates where the explosion"
+            " should take place (center)\nr3: explosion radius (only works correctly"
+            " with 1 and 2)\nstack[0]: damage type\nstack[1]: damage source (normally"
             " DAMAGE_SOURCE_EXPLOSION)"
         ),
     )
 
     TryWarp = Symbol(
         None,
         None,
@@ -19382,14 +20966,57 @@
     GetStairsRoom = Symbol(
         None,
         None,
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    UpdateTrapsVisibility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Exact purpose unknown. Gets called whenever a trap tile is shown or"
+            " hidden.\n\nNo params."
+        ),
+    )
+
+    DrawTileGrid = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Draws a grid on the nearby walkable tiles. Triggered by pressing Y.\n\nr0:"
+            " Coordinates of the entity around which the grid will be drawn\nr1: ?\nr2:"
+            " ?\nr3: ?"
+        ),
+    )
+
+    HideTileGrid = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Hides the grid on the nearby walkable tiles. Triggered by releasing"
+            " Y.\n\nNo params."
+        ),
+    )
+
+    DiscoverMinimap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Discovers the tiles around the specified position on the minimap.\n\nThe"
+            " discovery radius depends on the visibility range of the floor. If"
+            " display_data::blinded is true, the function returns early without doing"
+            " anything.\n\nr0: Position around which the map should be discovered"
+        ),
+    )
+
     IsWaterTileset = Symbol(
         None,
         None,
         None,
         (
             "Returns flag tileset_property::is_water_tileset for the current"
             " tileset\n\nreturn: True if the current tileset is a water tileset"
@@ -19455,14 +21082,34 @@
         (
             "Sets the boost_kecleon_shop_spawn_chance field on the dungeon struct"
             " depending on if a team member has the exclusive item effect for more"
             " kecleon shops.\n\nNo params."
         ),
     )
 
+    SetDoughSeedFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the dough_seed_extra_money_flag field on the dungeon struct to the"
+            " given value.\n\nr0: bool to set the flag to"
+        ),
+    )
+
+    TrySpawnDoughSeedPoke = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the dough_seed_extra_money_flag field on the dungeon struct and"
+            " tries to spawn\nextra poke if it is set.\n\nNo params."
+        ),
+    )
+
     IsSecretBazaar = Symbol(
         None,
         None,
         None,
         "Checks if the current floor is the Secret Bazaar.\n\nreturn: bool",
     )
 
@@ -19513,28 +21160,62 @@
         None,
         (
             "Checks if the current floor is a secret bazaar or a secret"
             " room.\n\nreturn: bool"
         ),
     )
 
+    HiddenStairsPresent = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the hidden stairs are present on this floor.\n\nThe function"
+            " checks that dungeon_generation_info::hidden_stairs_pos isn't (-1,"
+            " -1)\n\nreturn: True if the hidden stairs are present on this floor, false"
+            " otherwise."
+        ),
+    )
+
+    HiddenStairsTrigger = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called whenever the leader steps on the hidden stairs.\n\nIf the stairs"
+            " hadn't been revealed yet, plays the corresponding animation.\n\nr0: True"
+            " to display a message if the stairs are revealed, false to omit it."
+        ),
+    )
+
     GetDungeonGenInfoUnk0C = Symbol(
         None, None, None, "return: dungeon_generation_info::field_0xc"
     )
 
     GetMinimapData = Symbol(
         None,
         None,
         None,
         (
             "Returns a pointer to the minimap_display_data struct in the dungeon"
             " struct.\n\nreturn: minimap_display_data*"
         ),
     )
 
+    DrawMinimapTile = Symbol(
+        None,
+        None,
+        None,
+        "Draws a single tile on the minimap.\n\nr0: X position\nr1: Y position",
+    )
+
+    UpdateMinimap = Symbol(
+        None, None, None, "Graphically updates the minimap\n\nNo params."
+    )
+
     SetMinimapDataE447 = Symbol(
         None,
         None,
         None,
         (
             "Sets minimap_display_data::field_0xE447 to the specified value\n\nr0:"
             " Value to set the field to"
@@ -19558,14 +21239,35 @@
         None,
         (
             "Sets minimap_display_data::field_0xE448 to the specified value\n\nr0:"
             " Value to set the field to"
         ),
     )
 
+    InitWeirdMinimapMatrix = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the matrix at minimap_display_data+0xE000. Seems to overflow"
+            " said matrix when doing so.\n\nNo params."
+        ),
+    )
+
+    InitMinimapDisplayTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to initialize an instance of struct minimap_display_tile\n\nr0:"
+            " Pointer to struct to init\nr1: Seems to be a pointer to the file that"
+            " stores minimap icons or something like that"
+        ),
+    )
+
     LoadFixedRoomDataVeneer = Symbol(
         None,
         None,
         None,
         (
             "Likely a linker-generated veneer for LoadFixedRoomData.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nNo"
@@ -20257,14 +21959,24 @@
             " reached by the traversal algorithm, then the stairs must not be reachable"
             " from that tile.\n\nr0: x coordinate of the stairs\nr1: y coordinate of"
             " the stairs\nr2: flag to always return true, but set a special bit on all"
             " walkable tiles that aren't reachable from the stairs\nreturn: bool"
         ),
     )
 
+    GetNextFixedRoomAction = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the next action that needs to be performed when spawning a fixed"
+            " room tile.\n\nreturn: Next action ID"
+        ),
+    )
+
     ConvertWallsToChasms = Symbol(
         None, None, None, "Converts all wall tiles to chasms.\n\nNo params."
     )
 
     ResetInnerBoundaryTileRows = Symbol(
         None,
         None,
@@ -20315,25 +22027,75 @@
             " HIDDEN_STAIRS_RANDOM_SECRET_BAZAAR_OR_SECRET_ROOM and the"
             " floor_properties::hidden_stairs_spawn_chance) into a concrete hidden"
             " stairs type.\n\nr0: dungeon generation info pointer\nr1: floor properties"
             " pointer\nreturn: enum hidden_stairs_type"
         ),
     )
 
+    GetFinalKecleonShopSpawnChance = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the kecleon shop spawn chance for the floor.\n\nWhen"
+            " dungeon::boost_kecleon_shop_spawn_chance is false, returns the same value"
+            " as the input. When it's true, returns the input (chance * 1.2).\n\nr0:"
+            " base kecleon shop spawn chance,"
+            " floor_properties::kecleon_shop_spawn_chance\nreturn: int"
+        ),
+    )
+
     ResetHiddenStairsSpawn = Symbol(
         None,
         None,
         None,
         (
             "Resets hidden stairs spawn information for the floor. This includes the"
             " position on the floor generation status as well as the flag indicating"
             " whether the spawn was blocked.\n\nNo params."
         ),
     )
 
+    PlaceFixedRoomTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to spawn a single tile when generating a fixed room. The tile might"
+            " contain an item or a monster.\n\nr0: Pointer to the tile to spawn\nr1:"
+            " Fixed room action to perform. Controls what exactly will be spawned. The"
+            " action is actually 12 bits long, the highest 4 bits are used as a"
+            " parameter that represents a direction (for example, when spawning a"
+            " monster).\nr2: Tile X position\nr3: Tile Y position"
+        ),
+    )
+
+    FixedRoomActionParamToDirection = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Converts the parameter stored in a fixed room action value to a direction"
+            " ID.\n\nThe conversion is performed by subtracting 1 to the value. If the"
+            " parameter had a value of 0, DIR_NONE is returned.\n\nr0: Parameter"
+            " value\nreturn: Direction"
+        ),
+    )
+
+    ApplyKeyEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to open a locked door in front of the target if a locked door has"
+            " not already\nbeen open on the floor.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
     LoadFixedRoomData = Symbol(
         None,
         None,
         None,
         (
             "Loads fixed room data from BALANCE/fixed.bin into the buffer pointed to by"
             " FIXED_ROOM_DATA_PTR.\n\nNo params."
@@ -21107,15 +22869,27 @@
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
             " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
-    OpenMenu = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
+    OpenMenu = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Opens a menu. The menu to open depends on the specified parameter.\n\nIt"
+            " looks like the function takes a parameter in r0, but doesn't use it. r1"
+            " doesn't even get set when this function is called.\n\nr0: (?) Unused by"
+            " the function. Seems to be 1 byte long.\nr1: (?) Unused by the function."
+            " Seems to be 1 byte long.\nr2: True to open the bag menu, false to open"
+            " the main dungeon menu"
+        ),
+    )
 
     OthersMenuLoop = Symbol(
         None,
         None,
         None,
         (
             "Called on each frame while the in-dungeon 'others' menu is open.\n\nIt"
@@ -21290,27 +23064,27 @@
         None,
         (
             "The move target and range code for special healing moves that target just"
             " the user (0x273).\n\ntype: struct move_target_and_range (+ padding)"
         ),
     )
 
-    PLAIN_SEED_VALUE = Symbol(
-        None, None, None, "Some value related to the Plain Seed (0xBE9)."
+    PLAIN_SEED_STRING_ID = Symbol(
+        None, None, None, "The string ID for eating a Plain Seed (0xBE9)."
     )
 
     MAX_ELIXIR_PP_RESTORATION = Symbol(
         None,
         None,
         None,
         "The amount of PP restored per move by ingesting a Max Elixir (0x3E7).",
     )
 
-    SLIP_SEED_VALUE = Symbol(
-        None, None, None, "Some value related to the Slip Seed (0xC75)."
+    SLIP_SEED_FAIL_STRING_ID = Symbol(
+        None, None, None, "The string ID for when eating the Slip Seed fails (0xC75)."
     )
 
     ROCK_WRECKER_MOVE_ID = Symbol(
         None, None, None, "The move ID for Rock Wrecker (453)."
     )
 
     CASTFORM_NORMAL_FORM_MALE_ID = Symbol(
@@ -22055,15 +23829,28 @@
     loadaddress = None
     length = None
     functions = EuItcmOverlay3Functions
     data = EuItcmOverlay3Data
 
 
 class EuItcmOverlay30Functions:
-    pass
+    WriteQuicksaveData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Function responsible for writing dungeon data when quicksaving.\n\nAmong"
+            " other things, it contains a loop that goes through all the monsters in"
+            " the current dungeon, copying their data to the buffer. The data is not"
+            " copied as-is though, the game uses a reduced version of the monster"
+            " struct containing only the minimum required data to resume the game"
+            " later.\n\nr0: Pointer to buffer where data should be written\nr1: Buffer"
+            " size. Seems to be 0x5800 (22 KB) when the function is called."
+        ),
+    )
 
 
 class EuItcmOverlay30Data:
     OVERLAY30_JP_STRING_1 = Symbol(None, None, None, "みさき様")
 
     OVERLAY30_JP_STRING_2 = Symbol(None, None, None, "やよい様")
```

## pmdsky_debug_py/jp.py

```diff
@@ -1033,17 +1033,17 @@
 
     LoadFileInPackWithPackId = Symbol(
         [0xC35C],
         [0x200C35C],
         None,
         (
             "Call LoadFileInPack after looking up the global Pack archive by its"
-            " identifier\n\nr0: pack file identifier\nr1: [output] target buffer\nr2:"
-            " file index\nreturn: number of read bytes (identical to the length of the"
-            " pack from the Table of Content)"
+            " identifier\n\nr0: pack file identifier\nr1: file index\nr2: [output]"
+            " target buffer\nreturn: number of read bytes (identical to the length of"
+            " the pack from the Table of Content)"
         ),
     )
 
     AllocAndLoadFileInPack = Symbol(
         [0xC388],
         [0x200C388],
         None,
@@ -1084,14 +1084,27 @@
             "Load the indexed file from the Pack archive, itself loaded from the"
             " ROM.\n\nr0: pack file struct\nr1: [output] target buffer\nr2: file"
             " index\nreturn: number of read bytes (identical to the length of the pack"
             " from the Table of Content)"
         ),
     )
 
+    GetDungeonResultMsg = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the message that is shown on the dungeon results ('The Last Outing')"
+            " screen, right after the leader's name.\n\nr0: Damage source value to use"
+            " when displaying the cause of fainting or the result of the"
+            " expedition\nr1: [output] Buffer where the resulting message will be"
+            " stored\nr2: Buffer size\nr3: (?) Seems to point to a buffer"
+        ),
+    )
+
     GetDamageSource = Symbol(
         [0xCA54],
         [0x200CA54],
         None,
         (
             "Gets the damage source for a given move-item combination.\n\nIf there's no"
             " item, the source is the move ID. If the item is an orb, return"
@@ -1169,14 +1182,26 @@
         None,
         (
             "Checks if an item is one of the aura bows received at the start of the"
             " game.\n\nr0: item ID\nreturn: bool"
         ),
     )
 
+    IsTreasureBox = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the given item ID is a treasure box\n\nIn particular, it checks"
+            " if the category of the item is CATEGORY_TREASURE_BOXES_1,"
+            " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
+            " ID\nreturn: True if the item is a treasure box, false otherwise"
+        ),
+    )
+
     InitItem = Symbol(
         [0xCE9C],
         [0x200CE9C],
         None,
         (
             "Initialize an item struct with the given information.\n\nThis will resolve"
             " the quantity based on the item type. For Poké, the quantity code will"
@@ -1494,22 +1519,21 @@
     GetItemMoveId = Symbol(
         [0xEAB0],
         [0x200EAB0],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: move ID",
     )
 
-    TestItemFlag0xE = Symbol(
+    TestItemAiFlag = Symbol(
         [0xEAD0],
         [0x200EAD0],
         None,
         (
-            "Tests bit 7 if r1 is 0, bit 6 if r1 is 1, bit 5 otherwise\n\nNote:"
-            " unverified, ported from Irdkwia's notes\n\nr0: item ID\nr1:"
-            " bit_id\nreturn: bool"
+            "Used to check the AI flags for an item. Tests bit 7 if r1 is 0, bit 6 if"
+            " r1 is 1, bit\n5 otherwise.\n\nr0: item ID\nr1: bit_id\nreturn: bool"
         ),
     )
 
     IsItemInTimeDarkness = Symbol(
         [0xEB60],
         [0x200EB60],
         None,
@@ -1547,14 +1571,25 @@
         None,
         (
             "Sets the amount of money the player is carrying, clamping the value to the"
             " range [0, MAX_MONEY_CARRIED].\n\nr0: new value"
         ),
     )
 
+    AddMoneyCarried = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds the amount of money to the player's current amount of money. Just"
+            " calls\nSetMoneyCarried with the current money + money gained.\n\nr0:"
+            " money gained (can be negative)"
+        ),
+    )
+
     GetCurrentBagCapacity = Symbol(
         [0xEDB4],
         [0x200EDB4],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: bag capacity",
     )
 
@@ -1575,15 +1610,18 @@
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: # items",
     )
 
     CountNbItemsOfTypeInBag = Symbol(
         [0xEE7C],
         [0x200EE7C],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: count",
+        (
+            "Returns the number of items of the given kind in the bag\n\nr0: item"
+            " ID\nreturn: count"
+        ),
     )
 
     CountItemTypeInBag = Symbol(
         [0xEEB8],
         [0x200EEB8],
         None,
         (
@@ -1804,14 +1842,24 @@
     ScriptSpecialProcess0x39 = Symbol(
         [0xFD24],
         [0x200FD24],
         None,
         "Implements SPECIAL_PROC_0x39 (see ScriptSpecialProcessCall).\n\nreturn: bool",
     )
 
+    CountNbItemsOfTypeInStorage = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the number of items of the given kind in the storage\n\nr0: item"
+            " ID\nreturn: count"
+        ),
+    )
+
     CountItemTypeInStorage = Symbol(
         [0xFEB4],
         [0x200FEB4],
         None,
         (
             "Implements SPECIAL_PROC_COUNT_ITEM_TYPE_IN_STORAGE (see"
             " ScriptSpecialProcessCall).\n\nr0: pointer to an owned_item\nreturn:"
@@ -2673,38 +2721,62 @@
     )
 
     DeleteWanTableEntry = Symbol(
         [0x1D234],
         [0x201D234],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
+            "Always delete an entry if the file is allocated externally"
+            " (file_externally_allocated is set), otherwise, decrease the reference"
+            " counter. If it reach 0, delete the sprite.\n\nr0: wan_table_ptr\nr1:"
             " wan_id"
         ),
     )
 
+    AllocateWanTableEntry = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return the identifier to a free wan table entry (-1 if none are"
+            " avalaible). The entry is zeroed.\n\nr0: wan_table_ptr\nreturn: the entry"
+            " id in wan_table"
+        ),
+    )
+
     FindWanTableEntry = Symbol(
         [0x1D32C],
         [0x201D32C],
         None,
         (
-            "Appears to search in the given table (in practice always seems to be"
+            "Search in the given table (in practice always seems to be"
             " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
             " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
             " if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         [0x1D38C],
         [0x201D38C],
         None,
         (
-            "wan_id = -1 if it is not loaded\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: wan_table_ptr\nr1: bin_file_id\nr2: file_id\nreturn: wan_id"
+            "Look up a sprite with the provided pack_id and file_index in the wan"
+            " table.\n\nr0: wan_table_ptr\nr1: pack_id\nr2: file_index\nreturn: sprite"
+            " id in the wan table, -1 if not found"
+        ),
+    )
+
+    InitWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the input WAN table with 0x60 free entries (it needs a length"
+            " of 0x1510 bytes)\n\nr0: wan_table_ptr"
         ),
     )
 
     LoadWanTableEntry = Symbol(
         [0x1D434],
         [0x201D434],
         None,
@@ -2712,14 +2784,40 @@
             "Appears to load data from the given file (in practice always seems to be"
             " animation data), using previously loaded data in the given table (see"
             " FindWanTableEntry) if possible.\n\nr0: table pointer\nr1: file name\nr2:"
             " flags\nreturn: table index of the loaded data"
         ),
     )
 
+    LoadWanTableEntryFromPack = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3: allocation"
+            " flags\nstack[0]: compressed\nreturn: the entry id in wan_table"
+        ),
+    )
+
+    LoadWanTableEntryFromPackUseProvidedMemory = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite into the"
+            " provided memory area. Mark the sprite as externally allocated.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3:"
+            " sprite_storage_ptr\nstack[0]: compressed\nreturn: the entry id in"
+            " wan_table"
+        ),
+    )
+
     ReplaceWanFromBinFile = Symbol(
         [0x1D6DC],
         [0x201D6DC],
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
             " wan_id\nr2: bin_file_id\nr3: file_id\nstack[0]: compressed"
@@ -2978,14 +3076,30 @@
         [0x243B0], [0x20243B0], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetStringPower = Symbol(
         [0x24478], [0x2024478], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    GetDungeonResultString = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns a string containing some information to be used when displaying"
+            " the dungeon results screen.\n\nThe exact string returned depends on the"
+            " value of r0:\n0: Name of the move that fainted the leader. Empty string"
+            " if the leader didn't faint.\n1-3: Seems to always result in an empty"
+            " string.\n4: Name of the pokémon that fainted the leader, or name of the"
+            " leader if the leader didn't faint.\n5: Name of the fainted leader. Empty"
+            " string if the leader didn't faint.\n\nr0: String to return\nreturn:"
+            " Pointer to resulting string"
+        ),
+    )
+
     SetQuestionMarks = Symbol(
         [0x25134],
         [0x2025134],
         None,
         (
             "Fills the buffer with the string '???'\n\nNote: unverified, ported from"
             " Irdkwia's notes\n\nr0: buffer"
@@ -3311,15 +3425,15 @@
 
     IsMenuOptionActive = Symbol(
         [0x32794],
         [0x2032794],
         None,
         (
             "Called whenever a menu option is selected. Returns whether the option is"
-            " active or not.\n\nr0: ?\nReturn: True if the menu option is enabled,"
+            " active or not.\n\nr0: ?\nreturn: True if the menu option is enabled,"
             " false otherwise."
         ),
     )
 
     ShowKeyboard = Symbol(
         [0x36B08],
         [0x2036B08],
@@ -3703,14 +3817,24 @@
         None,
         (
             "Gets the special episode type from the SPECIAL_EPISODE_TYPE script"
             " variable.\n\nreturn: special episode type"
         ),
     )
 
+    GetExecuteSpecialEpisodeType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the special episode type from the EXECUTE_SPECIAL_EPISODE_TYPE script"
+            " variable.\n\nreturn: special episode type"
+        ),
+    )
+
     HasPlayedOldGame = Symbol(
         [0x4CDD0],
         [0x204CDD0],
         None,
         "Returns the value of the VAR_PLAY_OLD_GAME script variable.\n\nreturn: bool",
     )
 
@@ -3773,21 +3897,21 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: dungeon ID\nr1:"
             " bit_value"
         ),
     )
 
-    CheckDungeonOpen = Symbol(
+    GetDungeonMode = Symbol(
         [0x4D2FC],
         [0x204D2FC],
         None,
         (
-            "Related to dungeon open list\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: dungeon ID\nreturn: status code?"
+            "Returns the mode of the specified dungeon\n\nr0: Dungeon ID\nreturn:"
+            " Dungeon mode"
         ),
     )
 
     GlobalProgressAlloc = Symbol(
         [0x4D468],
         [0x204D468],
         None,
@@ -4000,14 +4124,59 @@
         (
             "If buffer_portrait is null, it only checks if it exists\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: portrait box pointer\nr1:"
             " buffer_portrait\nreturn: exists"
         ),
     )
 
+    SetEnterDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to set the dungeon that will be accessed when switching from ground"
+            " to dungeon mode.\n\nr0: Dungeon ID"
+        ),
+    )
+
+    InitDungeonInit = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the dungeon_init struct before entering a dungeon.\n\nr0:"
+            " [output] Pointer to the struct to init\nr1: Dungeon ID"
+        ),
+    )
+
+    IsNoLossPenaltyDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the specified dungeon shouldn't have a loss penalty.\n\nIf"
+            " true you won't lose your money and items upon fainting. Also used to"
+            " initialize dungeon_init::skip_faint_animation_flag.\n\nReturns: True for"
+            " DUNGEON_CRYSTAL_LAKE and DUNGEON_5TH_STATION_CLEARING, as well as for"
+            " DUNGEON_DEEP_STAR_CAVE_TEAM_ROGUE if the ground variable SIDE01_BOSS2ND"
+            " is 0; false otherwise."
+        ),
+    )
+
+    CheckMissionRestrictions = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Seems to be used to check if you have any missions that have unmet"
+            " restrictions when trying to access a dungeon.\n\nr0: ?\nreturn: (?) Seems"
+            " to be composed of multiple bitflags."
+        ),
+    )
+
     GetNbFloors = Symbol(
         [0x4F8D4],
         [0x204F8D4],
         None,
         (
             "Returns the number of floors of the given dungeon.\n\nThe result is"
             " hardcoded for certain dungeons, such as dojo mazes.\n\nr0: Dungeon"
@@ -4069,19 +4238,75 @@
         (
             "Given a dungeon ID and a floor number, returns a struct with the"
             " corresponding dungeon group and floor number in that group.\n\nThe"
             " function normally uses the data in mappa_s.bin to calculate the result,"
             " but there's some dungeons (such as dojo mazes) that have hardcoded return"
             " values.\n\nIrdkwia's notes:\n  [r1]: dungeon_id\n  [r1+1]:"
             " dungeon_floor_id\n  [r0]: group_id\n  [r0+1]: group_floor_id\n\nr0:"
-            " (output) Struct containing the dungeon group and floor group\nr1: Struct"
+            " [output] Struct containing the dungeon group and floor group\nr1: Struct"
             " containing the dungeon ID and floor number"
         ),
     )
 
+    GetMissionRank = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the mission rank for the given dungeon and floor.\n\nIf the dungeon"
+            " ID is >= DUNGEON_NORMAL_FLY_MAZE or the group of the dungeon is >"
+            " DGROUP_DUMMY_0x63, returns MISSION_RANK_E.\n\nr0: Dungeon and"
+            " floor\nreturn: Mission rank"
+        ),
+    )
+
+    GetOutlawLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for outlaws for the given dungeon and"
+            " floor\n\nr0: Dungeon and floor\nreturn: Outlaw level"
+        ),
+    )
+
+    GetOutlawLeaderLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for team leader outlaws for the given"
+            " dungeon and floor. Identical to GetOutlawLevel.\n\nr0: Dungeon and"
+            " floor\nreturn: Outlaw leader level"
+        ),
+    )
+
+    GetOutlawMinionLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for minion outlaws for the given"
+            " dungeon and floor.\n\nr0: Dungeon and floor\nreturn: Outlaw minion level"
+        ),
+    )
+
+    AddGuestMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds a guest monster to the active team\n\nr0: dungeon_init struct for the"
+            " dungeon that is about to be entered\nr1: Number of the guest monster to"
+            " add. Used when more than one monster is added.\nr2: Pointer to the guest"
+            " monster entry to add to the team (usually located within"
+            " GUEST_MONSTER_DATA)"
+        ),
+    )
+
     GetGroundNameId = Symbol(
         [0x4FCAC], [0x204FCAC], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetAdventureLogStructLocation = Symbol(
         [0x4FD70],
         [0x204FD70],
@@ -5179,14 +5404,24 @@
     LoadM2nAndN2m = Symbol(
         [0x52F0C],
         [0x2052F0C],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    GuestMonsterToGroundMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inits a ground_monster entry with the given guest_monster struct.\n\nr0:"
+            " [output] ground_monster struct to init\nr1: guest_monster struct to use"
+        ),
+    )
+
     StrcmpMonsterName = Symbol(
         [0x532E8],
         [0x20532E8],
         None,
         (
             "Checks if the string_buffer matches the name of the species\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: string_buffer\nr1: monster"
@@ -5758,15 +5993,15 @@
         [0x59000],
         [0x2059000],
         None,
         (
             "Determines the list of IQ skills that a given monster can learn given its"
             " IQ value.\n\nThe list of skills is written in the array specified in r0."
             " The array has 69 slots in total. Unused slots are set to 0.\n\nr0:"
-            " (output) Array where the list of skills will be written\nr1: Monster"
+            " [output] Array where the list of skills will be written\nr1: Monster"
             " species\nr2: Monster IQ\nreturn: Amount of skills written to the output"
             " array"
         ),
     )
 
     DisableIqSkill = Symbol(
         [0x590A0],
@@ -6213,14 +6448,29 @@
         (
             "Converts an index in DUNGEON_SWAP_ID_TABLE to the corresponding dungeon"
             " ID, or DUNGEON_DUMMY_0xFF if the index is -1.\n\nr0: index\nreturn:"
             " dungeon ID"
         ),
     )
 
+    GetDungeonModeSpecial = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the status of the given dungeon, with some modifications.\n\nIf"
+            " the dungeon ID is DUNGEON_BEACH, returns DMODE_REQUEST.\nIf it's"
+            " DUNGEON_JOINED_AT_UNKNOWN, returns DMODE_OPEN_AND_REQUEST.\nIf it's >="
+            " DUNGEON_NORMAL_FLY_MAZE and <= DUNGEON_DOJO_0xD3, returns"
+            " DMODE_OPEN_AND_REQUEST.\nElse, calls GetDungeonMode and returns"
+            " DMODE_REQUEST if the dungeon has been cleared, or DMODE_OPEN if it's"
+            " not.\n\nr0: Dungeon ID\nreturn: Dungeon mode"
+        ),
+    )
+
     ResumeBgm = Symbol(
         [0x6DCA4],
         [0x206DCA4],
         None,
         "Uncertain.\n\nNote: unverified, ported from Irdkwia's notes",
     )
 
@@ -6231,14 +6481,94 @@
     UpdateChannels = Symbol(
         [0x74774],
         [0x2074774],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    ClearIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enables processor interrupts by clearing the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were disabled, 0x0 if they were already enabled)"
+        ),
+    )
+
+    EnableIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Disables processor interrupts by setting the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were already disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    SetIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the value of the processor's interrupt flag according to the"
+            " specified parameter.\n\nr0: Value to set the flag to (0x80 to set it,"
+            " which disables interrupts; 0x0 to unset it, which enables"
+            " interrupts)\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts were"
+            " disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    EnableIrqFiqFlags = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Disables processor all interrupts (both standard and fast) by setting the"
+            " i and f flags in the program status register (cpsr).\n\nreturn: Old value"
+            " of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    SetIrqFiqFlags = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the value of the processor's interrupt flags (i and f) according to"
+            " the specified parameter.\n\nr0: Value to set the flags to (0xC0 to set"
+            " both flags, 0x80 to set the i flag and clear the f flag, 0x40 to set the"
+            " f flag and clear the i flag and 0x0 to clear both flags)\nreturn: Old"
+            " value of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    GetIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the current value of the processor's interrupt request (i)"
+            " flag\n\nreturn: cpsr & 0x80 (0x80 if interrupts are disabled, 0x0 if they"
+            " are enabled)"
+        ),
+    )
+
+    WaitForever2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EnableIrqFlag and WaitForInterrupt in an infinite loop.\n\nThis is"
+            " called on fatal errors to hang the program indefinitely.\n\nNo params."
+        ),
+    )
+
     WaitForInterrupt = Symbol(
         [0x7BF18],
         [0x207BF18],
         None,
         (
             "Presumably blocks until the program receives an interrupt.\n\nThis just"
             " calls (in Ghidra terminology) coproc_moveto_Wait_for_interrupt(0). See"
@@ -12848,14 +13178,24 @@
         None,
         (
             "The multiplier for damage from the Air Blade (1.5), as a binary"
             " fixed-point number (8 fraction bits)"
         ),
     )
 
+    KECLEON_SHOP_BOOST_CHANCE_MULTIPLIER = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The boosted kecleon shop spawn chance multiplier (~1.2) as a binary"
+            " fixed-point number (8 fraction bits)."
+        ),
+    )
+
     HIDDEN_STAIRS_SPAWN_CHANCE_MULTIPLIER = Symbol(
         None,
         None,
         None,
         (
             "The hidden stairs spawn chance multiplier (~1.2) as a binary fixed-point"
             " number (8 fraction bits), if applicable. See"
@@ -13536,16 +13876,18 @@
     )
 
     LoadBackgroundAttributes = Symbol(
         [0xF894],
         [0x22ED174],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: [output]"
-            " bg_attr_str\nr1: bg_id"
+            "Open and read an entry from the MAP_BG/bg_list.dat\n\nDocumentation on"
+            " this format can be found"
+            " here:\nhttps://github.com/SkyTemple/skytemple-files/tree/55b3017631a8a1b0f106111ef91a901dc394c6df/skytemple_files/graphics/bg_list_dat\n\nr0:"
+            " [output] The entry\nr1: background ID"
         ),
     )
 
     LoadMapType10 = Symbol(
         [0x10A78],
         [0x22EE358],
         None,
@@ -13648,14 +13990,24 @@
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
             " characters printed, excluding the null-terminator"
         ),
     )
 
+    GetExclusiveItemRequirements = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to calculate the items required to get a certain exclusive item in"
+            " the swap shop.\n\nr0: ?\nr1: ?"
+        ),
+    )
+
     StatusUpdate = Symbol(
         [0x3771C],
         [0x2314FFC],
         None,
         (
             "Implements SPECIAL_PROC_STATUS_UPDATE (see"
             " ScriptSpecialProcessCall).\n\nNo params."
@@ -13814,14 +14166,18 @@
         ),
     )
 
     UNIONALL_RAM_ADDRESS = Symbol(None, None, None, "[Runtime]")
 
     GROUND_STATE_MAP = Symbol(None, None, None, "[Runtime]")
 
+    GROUND_STATE_WEATHER = Symbol(
+        None, None, None, "[Runtime] Same structure format as GROUND_STATE_MAP"
+    )
+
     GROUND_STATE_PTRS = Symbol(
         None,
         None,
         None,
         (
             "Host pointers to multiple structure used for performing an overworld"
             " scene\n\ntype: struct main_ground_data"
@@ -15677,24 +16033,81 @@
     FadeToBlack = Symbol(
         [0x4718],
         [0x22E1FF8],
         None,
         "Fades the screen to black across several frames.\n\nNo params.",
     )
 
+    CheckTouchscreenArea = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the currently pressed touchscreen position is within the"
+            " specified area.\n\nr0: Area lower X coordinate\nr1: Area lower Y"
+            " coordinate\nr2: Area upper X coordinate\nr3: Area upper Y"
+            " coordinate\nreturn: True if the specified area contains the currently"
+            " pressed touchscreen position, false otherwise."
+        ),
+    )
+
+    GetTrapInfo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Given a trap entity, returns the pointer to the trap info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Trap data pointer"
+        ),
+    )
+
+    GetItemInfo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Given an item entity, returns the pointer to the item info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Item data pointer"
+        ),
+    )
+
     GetTileAtEntity = Symbol(
         [0x53D8],
         [0x22E2CB8],
         None,
         (
             "Returns a pointer to the tile where an entity is located.\n\nr0: pointer"
             " to entity\nreturns: pointer to tile"
         ),
     )
 
+    UpdateEntityPixelPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Updates an entity's pixel_pos field using the specified pixel_position"
+            " struct, or its own pos field if it's null.\n\nr0: Entity pointer\nr1:"
+            " Pixel position to use, or null to use the entity's own position"
+        ),
+    )
+
+    CreateEnemyEntity = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Creates and initializes the entity struct of a newly spawned enemy"
+            " monster. Fails if there's 16 enemies on the floor already.\n\nIt could"
+            " also be used to spawn fixed room allies, since those share their slots on"
+            " the entity list.\n\nr0: Monster ID\nreturn: Pointer to the newly"
+            " initialized entity, or null if the entity couldn't be initialized"
+        ),
+    )
+
     SpawnTrap = Symbol(
         [0x6010],
         [0x22E38F0],
         None,
         (
             "Spawns a trap on the floor. Fails if there are more than 64 traps already"
             " on the floor.\n\nThis modifies the appropriate fields on the dungeon"
@@ -15714,35 +16127,46 @@
             " items already on the floor.\n\nThis initializes a new entry in the entity"
             " table and points it to the corresponding slot in the item info"
             " list.\n\nr0: position\nreturn: entity pointer for the newly added item,"
             " or null on failure"
         ),
     )
 
-    ShouldDisplayEntityMessages = Symbol(
+    ShouldMinimapDisplayEntity = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if a given entity should be displayed on the minimap\n\nr0: Entity"
+            " pointer\nreturn: True if the entity should be displayed on the minimap"
+        ),
+    )
+
+    ShouldDisplayEntity = Symbol(
         None,
         None,
         None,
         (
-            "Checks if messages that involve a certain entity should be displayed or"
-            " suppressed.\n\nFor example, it returns false if the entity is an"
-            " invisible enemy.\n\nr0: Entity pointer\nr1: ?\nreturn: True if messages"
-            " involving the entity should be displayed, false if they should be"
-            " suppressed."
+            "Checks if an entity should be displayed or not.\n\nFor example, it returns"
+            " false if the entity is an invisible enemy.\nAlso used to determine if"
+            " messages that involve a certain entity should be displayed or"
+            " suppressed.\n\nr0: Entity pointer\nr1: (?) Seems to be 1 for monsters and"
+            " 0 for items.\nreturn: True if the entity and its associated messages"
+            " should be displayed, false if they shouldn't."
         ),
     )
 
-    ShouldDisplayEntityMessagesWrapper = Symbol(
+    ShouldDisplayEntityWrapper = Symbol(
         None,
         None,
         None,
         (
-            "Calls ShouldDisplayEntityMessages with r1 = 0\n\nr0: Entity"
-            " pointer\nreturn: True if messages involving the entity should be"
-            " displayed, false if they should be suppressed."
+            "Calls ShouldDisplayEntity with r1 = 0\n\nr0: Entity pointer\nreturn: True"
+            " if the entity and its associated messages should be displayed, false if"
+            " they shouldn't."
         ),
     )
 
     CanSeeTarget = Symbol(
         [0x6500],
         [0x22E3DE0],
         None,
@@ -15862,28 +16286,54 @@
         (
             "Returns dungeon::display_data::visibility_range. If the visibility range"
             " is 0, returns 2 instead.\n\nreturn: Visibility range of the current"
             " floor, or 2 if the visibility is 0."
         ),
     )
 
-    PlayEffectAnimation = Symbol(
+    PlayEffectAnimationEntity = Symbol(
         [0x7374],
         [0x22E4C54],
         None,
         (
             "Just a guess. This appears to be paired often with"
             " GetEffectAnimationField0x19, and also has calls AnimationHasMoreFrames in"
             " a loop alongside AdvanceFrame(66) calls.\n\nThe third parameter skips the"
             " loop entirely. It seems like in this case the function might just preload"
-            " some animation frames for later use??\n\nr0: entity pointer\nr1: ?\nr2:"
-            " appears to be a flag for actually running the animation now? If this is"
-            " 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn: status"
-            " code, or maybe the number of frames or something? Either way, -1 seems to"
-            " indicate the animation being finished or something?"
+            " some animation frames for later use??\n\nr0: entity pointer\nr1: Effect"
+            " ID\nr2: appears to be a flag for actually running the animation now? If"
+            " this is 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn:"
+            " status code, or maybe the number of frames or something? Either way, -1"
+            " seems to indicate the animation being finished or something?"
+        ),
+    )
+
+    PlayEffectAnimationPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Takes a position struct in r0 and converts it to a pixel position struct"
+            " before calling PlayEffectAnimationPixelPos\n\nr0: Position where the"
+            " effect should be played\nr1: Effect ID\nr2: Unknown flag (same as the one"
+            " in PlayEffectAnimationEntity)\nreturn: Result of call to"
+            " PlayEffectAnimationPixelPos"
+        ),
+    )
+
+    PlayEffectAnimationPixelPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Seems like a variant of PlayEffectAnimationEntity that uses pixel"
+            " coordinates as its first parameter instead of an entity pointer.\n\nr0:"
+            " Pixel position where the effect should be played\nr1: Effect ID\nr2:"
+            " Unknown flag (same as the one in PlayEffectAnimationEntity)\nreturn: Same"
+            " as PlayEffectAnimationEntity"
         ),
     )
 
     UpdateStatusIconFlags = Symbol(
         [0x7844],
         [0x22E5124],
         None,
@@ -15971,15 +16421,15 @@
         None,
         None,
         (
             "Copies all entries in the floor's monster spawn list that have a sprite"
             " size >= 6 to the specified buffer.\n\nThe parameter in r1 can be used to"
             " specify how many entries are already present in the buffer. Entries added"
             " by this function will be placed after those, and the total returned in r1"
-            " will account for existing entries as well.\n\nr0: (output) Buffer where"
+            " will account for existing entries as well.\n\nr0: [output] Buffer where"
             " the result will be stored\nr1: Current amount of entries in the"
             " buffer\nreturn: New amount of entries in the buffer"
         ),
     )
 
     IsOnMonsterSpawnList = Symbol(
         [0xBAD4],
@@ -16351,14 +16801,26 @@
             " the effect of the Switcher Orb). \n\nThe function checks for the Suction"
             " Cups ability for both the user and the target, and for the Mold Breaker"
             " ability on the user.\n\nr0: pointer to user entity\nr1: pointer to target"
             " entity"
         ),
     )
 
+    SetLeaderActionFields = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the leader's monster::action::action_id to the specified"
+            " value.\n\nAlso sets monster::action::action_use_idx and"
+            " monster::action::field_0xA to 0, as well as monster::action::field_0x10"
+            " and monster::action::field_0x12 to -1.\n\nr0: ID of the action to set"
+        ),
+    )
+
     ClearMonsterActionFields = Symbol(
         [0xF17C],
         [0x22ECA5C],
         None,
         (
             "Clears the fields related to AI in the monster's data struct, setting them"
             " all to 0.\nSpecifically, monster::action::action_id,"
@@ -16438,14 +16900,27 @@
         (
             "Sets a monster's action to action::ACTION_REGULAR_ATTACK, with a specified"
             " direction.\n\nr0: Pointer to the monster's action field\nr1: Direction in"
             " which to use the move. Gets stored in monster::action::direction."
         ),
     )
 
+    SetActionUseMovePlayer = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets a monster's action to action::ACTION_USE_MOVE_PLAYER, with a"
+            " specified monster and move index.\n\nr0: Pointer to the monster's action"
+            " field\nr1: Index of the monster that is using the move on the entity"
+            " list. Gets stored in monster::action::action_use_idx.\nr2: Index of the"
+            " move to use (0-3). Gets stored in monster::action::field_0xA."
+        ),
+    )
+
     SetActionUseMoveAi = Symbol(
         [0xFA44],
         [0x22ED324],
         None,
         (
             "Sets a monster's action to action::ACTION_USE_MOVE_AI, with a specified"
             " direction and move index.\n\nr0: Pointer to the monster's action"
@@ -16592,14 +17067,169 @@
             "If the flag for a trapper trap is set, handles spawning a trap based upon"
             " the\ninformation inside the dungeon struct. Uses the entity for logging a"
             " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
             " true if a trap was spawned succesfully"
         ),
     )
 
+    TryTriggerTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called whenever a monster steps on a trap.\n\nThe function will try to"
+            " trigger it. Nothing will happen if the pokémon has the same team as the"
+            " trap. The attempt to trigger the trap can also fail due to IQ skills, due"
+            " to the trap failing to work (random chance), etc.\n\nr0: Entity who"
+            " stepped on the trap\nr1: Trap position\nr2: ?\nr3: ?"
+        ),
+    )
+
+    ApplyMudTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly lowers attack, special attack, defense, or special defense of the"
+            " defender by 3 stages.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer"
+        ),
+    )
+
+    ApplyStickyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to make something in the bag"
+            " sticky. Otherwise, try to make the item the monster is holding"
+            " sticky.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyGrimyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to turn food items in the"
+            " toolbox into\ngrimy food. Otherwise, try to make the food item the"
+            " monster is holding grimy food.\n\nr0: attacker entity pointer\nr1:"
+            " defender entity pointer"
+        ),
+    )
+
+    ApplyPitfallTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, end the current floor unless it has a"
+            " rescue point.\nOtherwise, make the entity faint and ignore reviver seeds."
+            " If not called by a random\ntrap, break the grate on the pitfall"
+            " trap.\n\nr0: attacker entity pointer\nr1: defender entity pointer\nr2:"
+            " tile pointer\nr3: bool caused by random trap"
+        ),
+    )
+
+    ApplySummonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly spawns 2-4 enemy monsters around the position. The entity is only"
+            " used for\nlogging messages.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyPpZeroTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the PP of one of the defender's moves to 0.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyPokemonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Turns item in the same room as the tile at the position (usually just the"
+            " entities's\nposition) into monsters. If the position is in a hallway,"
+            " convert items in a 3x3 area\ncentered on the position into"
+            " monsters.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTripTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to drop the defender's item and places it on the floor.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyToxicSpikesTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to inflict 10 damage on the defender and then tries to poison"
+            " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyRandomTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Selects a random trap that isn't a wonder tile and isn't a random trap and"
+            " calls\nApplyTrapEffect on all monsters that is different from the trap's"
+            " team.\n\nr0: Triggered trap\nr1: User\nr2: Target, normally same as"
+            " user\nr3: Tile that contains the trap\nstack[0]: position"
+        ),
+    )
+
+    ApplyGrudgeTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Spawns several monsters around the position and gives all monsters on the"
+            " floor the\ngrudge status condition.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Performs the effect of a triggered trap.\n\nThe trap's animation happens"
+            " before this function is called.\n\nr0: Triggered trap\nr1: User\nr2:"
+            " Target, normally same as user\nr3: Tile that contains the trap\nstack[0]:"
+            " position\nstack[1]: trap ID\nstack[2]: bool caused by random"
+            " trap\nreturn: True if the trap should be destroyed after the effect is"
+            " applied"
+        ),
+    )
+
+    RevealTrapsNearby = Symbol(
+        None,
+        None,
+        None,
+        "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x13790],
         [0x22F1070],
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16623,28 +17253,63 @@
         None,
         (
             "Returns a pointer to the action data of the current leader (field 0x4A on"
             " its monster struct).\n\nNo params."
         ),
     )
 
+    GetEntityTouchscreenArea = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the area on the touchscreen that contains the sprite of the"
+            " specified entity\n\nr0: Entity pointer\nr1: [output] struct where the"
+            " result should be written"
+        ),
+    )
+
     SetLeaderAction = Symbol(
         [0x14BFC],
         [0x22F24DC],
         None,
         (
             "Sets the leader's action field depending on the inputs given by the"
             " player.\n\nThis function also accounts for other special situations that"
             " can force a certain action, such as when the leader is running. The"
             " function also takes care of opening the main menu when X is pressed.\nThe"
             " function generally doesn't return until the player has an action"
             " set.\n\nNo params."
         ),
     )
 
+    ShouldLeaderKeepRunning = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Determines if the leader should keep running. Returns false if the leader"
+            " bumps into something, or if an action that should stop the leader takes"
+            " place.\n\nreturn: True if the leader should keep running, false if it"
+            " should stop."
+        ),
+    )
+
+    CheckLeaderTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the tile the leader just stepped on and performs any required"
+            " actions, such as picking up items, triggering traps, etc.\n\nContains a"
+            " switch that checks the type of the tile the leader just stepped on.\n\nNo"
+            " params."
+        ),
+    )
+
     ChangeLeader = Symbol(
         [0x1764C],
         [0x22F4F2C],
         None,
         (
             "Tries to change the current leader to the monster specified by"
             " dungeon::new_leader.\n\nAccounts for situations that can prevent changing"
@@ -16787,14 +17452,25 @@
         (
             "Handles a fainted pokémon (reviving does not count as fainting).\n\nr0:"
             " Fainted entity\nr1: Damage source (move ID or greater than the max move"
             " id for other causes)\nr2: Entity responsible of the fainting"
         ),
     )
 
+    MoveMonsterToPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Moves a monster to the target position. Used both for regular movement and"
+            " special movement (like teleportation).\n\nr0: Entity pointer\nr1: X"
+            " target position\nr2: Y target position\nr3: ?"
+        ),
+    )
+
     UpdateAiTargetPos = Symbol(
         [0x1CE28],
         [0x22FA708],
         None,
         (
             "Given a monster, updates its target_pos field based on its current"
             " position and the direction in which it plans to attack.\n\nr0: Entity"
@@ -16919,14 +17595,24 @@
             "Restores PP for all moves, clears flags move::f_consume_2_pp,"
             " move::flags2_unk5 and move::flags2_unk7, and sets flag"
             " move::f_consume_pp.\nCalled when a monster is revived.\n\nr0: pointer to"
             " entity whose moves will be restored"
         ),
     )
 
+    BoostIQ = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's IQ.\n\nr0: monster entity pointer\nr1: iq"
+            " boost\nr2: bool suppress logs"
+        ),
+    )
+
     ShouldMonsterHeadToStairs = Symbol(
         [0x1E0F8],
         [0x22FB9D8],
         None,
         (
             "Checks if a given monster should try to reach the stairs when controlled"
             " by the AI\n\nr0: Entity pointer\nreturn: True if the monster should try"
@@ -16943,14 +17629,28 @@
             " dungeon::mew_cannot_spawn or the second parameter are true.\n\nCalled"
             " before spawning an enemy, appears to be checking if Mew can spawn on the"
             " current floor.\n\nr0: monster id\nr1: return false if the monster id is"
             " Mew\nreturn: bool"
         ),
     )
 
+    TryEndStatusWithAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if any of the defender's active abilities would end one of their"
+            " current status\nconditions. For example, if the ability Own Tempo will"
+            " stop confusion.\n\nCalled after changing a monster's ability with skill"
+            " swap, role play, or trace to\nremove statuses the monster should no"
+            " longer be affected by.\n\nr0: attacker entity pointer\nr1: defender"
+            " entity pointer"
+        ),
+    )
+
     ExclusiveItemEffectIsActive = Symbol(
         [0x383E0, 0x6BD58],
         [0x2315CC0, 0x2349638],
         None,
         (
             "Checks if a monster is a team member under the effects of a certain"
             " exclusive item effect.\n\nr0: entity pointer\nr1: exclusive item effect"
@@ -17080,14 +17780,27 @@
             "Checks if a monster does not gain experience.\n\nThis basically just"
             " inverts IsSpecialStoryAlly, with the exception of also checking for the"
             " 'Joined At' field being DUNGEON_CLIENT (is this set for mission"
             " clients?).\n\nr0: monster pointer\nreturn: bool"
         ),
     )
 
+    InitOtherMonsterData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes stats, IQ skills and moves for a given monster\n\nMight only"
+            " be used when spawning fixed room monsters.\n\nr0: Entity pointer\nr1:"
+            " Fixed room monster stats index\nr2: Spawn direction? (when calling this"
+            " function while spawning a fixed room monster, this is the parameter value"
+            " associated to the spawn action, after converting it to a direction.)"
+        ),
+    )
+
     SpawnTeam = Symbol(
         [0x2001C],
         [0x22FD8FC],
         None,
         "Seems to initialize and spawn the team when entering a dungeon.\n\nr0: ?",
     )
 
@@ -17127,20 +17840,32 @@
             " to the struct containing the data of the team member to"
             " initialize\nstack[0]: ?\nstack[1]: ?\nstack[2]: ?\nstack[3]:"
             " ?\nstack[4]: ?"
         ),
     )
 
     InitMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the monster struct within the provided entity struct.\n\nr0:"
+            " ?\nr1: Pointer to the entity whose monster struct should be"
+            " initialized\nr2: pointer to the entity's spawned_monster_data struct\nr3:"
+            " (?) Pointer to something"
+        ),
+    )
+
+    SubInitMonster = Symbol(
         [0x218D0],
         [0x22FF1B0],
         None,
         (
-            "Initializes a monster struct.\n\nr0: pointer to monster to initialize\nr1:"
-            " some flag"
+            "Called by InitMonster. Initializes some fields on the monster"
+            " struct.\n\nr0: pointer to monster to initialize\nr1: some flag"
         ),
     )
 
     MarkShopkeeperSpawn = Symbol(
         [0x21CA0],
         [0x22FF580],
         None,
@@ -17245,14 +17970,24 @@
         (
             "Returns the number of attacks that a monster can do in one turn (1 or"
             " 2).\n\nChecks for the abilities Swift Swim, Chlorophyll, Unburden, and"
             " for exclusive items.\n\nr0: pointer to entity\nreturns: int"
         ),
     )
 
+    GetMonsterDisplayNameType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Determines how the name of a monster should be displayed.\n\nr0: Entity"
+            " pointer\nreturn: Display name type"
+        ),
+    )
+
     GetMonsterName = Symbol(
         [0x23C58],
         [0x2301538],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: buffer\nr1: TargetInfo",
     )
 
@@ -17403,14 +18138,39 @@
         None,
         (
             "Checks if a monster has the sleep, nightmare, or napping status.\n\nr0:"
             " entity pointer\nreturn: bool"
         ),
     )
 
+    CanMonsterMoveInDirection = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the given monster can move in the specified direction\n\nReturns"
+            " false if any monster is standing on the target tile\n\nr0: Monster entity"
+            " pointer\nr1: Direction to check\nreturn: bool"
+        ),
+    )
+
+    GetFinalMobilityType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the mobility type of a monster, after accounting for things that"
+            " could affect it (like items or IQ skills)\n\nIf the specified direction"
+            " is DIR_NONE, direction checks are skipped. If it's not,"
+            " MOBILITY_INTANGIBLE is only returned if the direction is not"
+            " diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility type\nr2:"
+            " Direction of mobility\nreturn: Final mobility type"
+        ),
+    )
+
     IsMonsterCornered = Symbol(
         [0x24C3C],
         [0x230251C],
         None,
         (
             "True if the given monster is cornered (it can't move in any"
             " direction)\n\nr0: Entity pointer\nreturn: True if the monster can't move"
@@ -17438,15 +18198,15 @@
         [0x23027B8],
         None,
         (
             "Checks whether an AI-controlled monster can move in the specified"
             " direction.\nAccounts for walls, other monsters on the target position and"
             " IQ skills that might prevent a monster from moving into a specific"
             " location, such as House Avoider, Trap Avoider or Lava Evader.\n\nr0:"
-            " Entity pointer\nr1: Direction\nr2: (output) True if movement was not"
+            " Entity pointer\nr1: Direction\nr2: [output] True if movement was not"
             " possible because there was another monster on the target tile, false"
             " otherwise.\nreturn: True if the monster can move in the specified"
             " direction, false otherwise."
         ),
     )
 
     ShouldMonsterRunAway = Symbol(
@@ -17466,14 +18226,47 @@
         (
             "Calls ShouldMonsterRunAway and returns its result. It also calls another"
             " function if the result was true.\n\nr0: Entity pointer\nr1: ?\nreturn:"
             " Result of the call to ShouldMonsterRunAway"
         ),
     )
 
+    SafeguardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Safeguard.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: flag to log a message\nreturn:"
+            " bool"
+        ),
+    )
+
+    LeafGuardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is protected by the ability Leaf Guard.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer\nr2: flag to log a"
+            " message\nreturn: bool"
+        ),
+    )
+
+    IsProtectedFromStatDrops = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting their stats dropped"
+            " by the user.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     NoGastroAcidStatus = Symbol(
         [0x25954],
         [0x2303234],
         None,
         (
             "Checks if a monster does not have the Gastro Acid status.\n\nr0: entity"
             " pointer\nreturn: bool"
@@ -17634,14 +18427,25 @@
             "Updates monster::state_flags and monster::prev_state_flags with new"
             " values.\n\nr0: monster pointer\nr1: bitmask for bits to update\nr2:"
             " whether to set the bits indicated by the mask to 1 or 0\nreturn: whether"
             " or not any of the masked bits changed from the previous state"
         ),
     )
 
+    IsProtectedFromNegativeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting a negative status"
+            " condition.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     AddExpSpecial = Symbol(
         [0x261AC],
         [0x2303A8C],
         None,
         (
             "Adds to a monster's experience points, subject to experience boosting"
             " effects.\n\nThis function appears to be called only under special"
@@ -17655,17 +18459,31 @@
     )
 
     EnemyEvolution = Symbol(
         [0x2636C],
         [0x2303C4C],
         None,
         (
-            "Checks if the specified enemy should evolve because it just defeated an"
-            " ally, and if so, attempts to evolve it.\n\nr0: Pointer to the enemy to"
-            " check"
+            "Checks if any enemies on the floor should evolve and attempts to evolve"
+            " it. The\nentity pointer passed seems to get replaced by a generic"
+            " placeholder entity if the\nentity pointer passed is invalid.\n\nr0:"
+            " entity pointer"
+        ),
+    )
+
+    LevelUpItemEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to level up the the target. Calls LevelUp with a few extra checks"
+            " and messages\nfor using as an item. Used for the Joy Seed and Golden"
+            " Seed.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: number"
+            " of levels\nr3: bool message flag?\nstack[0]: bool show level up dialog"
+            " (for example 'Hey, I leveled up!' with a portrait)?"
         ),
     )
 
     TryDecreaseLevel = Symbol(
         [0x26BF4],
         [0x23044D4],
         None,
@@ -17677,27 +18495,31 @@
     )
 
     LevelUp = Symbol(
         [0x26CA8],
         [0x2304588],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: user entity"
-            " pointer\nr1: target entity pointer\nr2: message flag?\nr3: ?\nreturn:"
-            " success flag?"
+            "Attempts to level up the the target. Fails if the target's level can't be"
+            " raised. The show show level up dialog bool does nothing for monsters not"
+            " on the team.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " bool message flag?\nr3: bool show level up dialog (for example 'Hey, I"
+            " leveled up!' with a portrait)?\nreturn: success flag"
         ),
     )
 
     EvolveMonster = Symbol(
         [0x278EC],
         [0x23051CC],
         None,
         (
-            "Makes the specified monster evolve into the specified species.\n\nr0:"
-            " Pointer to the entity to evolve\nr1: ?\nr2: Species to evolve into"
+            "Makes the specified monster evolve into the specified species. Has a"
+            " special case when\na monster evolves into Ninjask and tries to spawn a"
+            " Shedinja as well.\n\nr0: user entity pointer?\nr1: target pointer to the"
+            " entity to evolve\nr2: Species to evolve into"
         ),
     )
 
     GetSleepAnimationId = Symbol(
         [0x28724],
         [0x2306004],
         None,
@@ -17719,14 +18541,58 @@
             " example, this delayed display system is used to display multiple monsters"
             " moving at once even though they take turns sequentially.\n\nr0: Pointer"
             " to an entity. Can be null.\nreturns: Seems to be true if there were any"
             " pending actions to display."
         ),
     )
 
+    CheckNonLeaderTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Similar to CheckLeaderTile, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: Entity pointer"
+        ),
+    )
+
+    EndNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Cures the target's negative status conditions. The game rarely (if not"
+            " never) calls\nthis function with the bool to remove the wrapping status"
+            " false.\n\nr0: pointer to user\nr1: pointer to target\nr2: bool play"
+            " animation\nr3: bool log failure message\nstack[0]: bool remove wrapping"
+            " status\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    EndNegativeStatusConditionWrapper = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EndNegativeStatusCondition with remove wrapping status false.\n\nr0:"
+            " pointer to user\nr1: pointer to target\nr2: bool play animation\nr3: bool"
+            " log failure message\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    TransferNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Transfers all negative status conditions the user has and gives then to"
+            " the target.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     EndSleepClassStatus = Symbol(
         None,
         None,
         None,
         (
             "Cures the target's sleep, sleepless, nightmare, yawn or napping status due"
             " to the action of the user, and prints the event to the log.\n\nr0:"
@@ -17832,14 +18698,25 @@
         (
             "Removes the target's magnet rise status due to the action of the user, and"
             " prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
             " target"
         ),
     )
 
+    TransferNegativeBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to transfer the the negative blinker class status conditions from"
+            " the user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer\nreturn: Whether or not the status could be transferred"
+        ),
+    )
+
     TryTriggerMonsterHouse = Symbol(
         [0x2BBA0],
         [0x2309480],
         None,
         (
             "Triggers a Monster House for an entity, if the right conditions are"
             " met.\n\nConditions: entity is valid and on the team, the tile is a"
@@ -18267,14 +19144,26 @@
         (
             "Inflicts the Sleep status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
             " number of turns\nr3: flag to log a message on failure"
         ),
     )
 
+    IsProtectedFromSleepClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is immune to sleep class status conditions.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nr2: ignore safeguard\nr3:"
+            " ignore other protections (exclusive items + leaf guard)\nstack[0]: flag"
+            " to log a message on failure\nreturn: bool"
+        ),
+    )
+
     TryInflictNightmareStatus = Symbol(
         [0x35878],
         [0x2313158],
         None,
         (
             "Inflicts the Nightmare status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
@@ -18777,91 +19666,638 @@
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
             " to log a message on failure\nr3: flag to only perform the check for"
             " inflicting without actually inflicting\nreturn: Whether or not the status"
             " could be inflicted"
         ),
     )
 
-    TryInflictDestinyBond = Symbol(
+    TryInflictDestinyBondStatus = Symbol(
         [0x39648],
         [0x2316F28],
         None,
         (
             "Inflicts the Destiny Bond status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
-    TryInvisify = Symbol(
+    TryInflictSureShotStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Sure Shot status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWhifferStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Whiffer status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSetDamageStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Set Damage status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictFocusEnergyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Focus Energy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictDecoyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Decoy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictCurseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Curse status condition on a target monster if possible and if"
+            " the user is\na ghost type. Otherwise, just boost the user's defense and"
+            " attack then lower the user's\nspeed.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
+    TryInflictSnatchStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Snatch status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictTauntStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Taunt status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictStockpileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Stockpile condition on a target monster if possible. Won't"
+            " boost the level\nof stockpiling above 3.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nreturn: Whether or not the status could be"
+            " inflicted or boosted"
+        ),
+    )
+
+    TryInflictInvisibleStatus = Symbol(
         None,
         None,
         None,
         (
             "Attempts to turn the target invisible.\n\nThe user pointer is only used"
             " when calling LogMessage functions.\n\nr0: user entity pointer\nr1: target"
             " entity pointer"
         ),
     )
 
+    TryInflictPerishSongStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Perish Song status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEncoreStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Encore status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryDecreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the belly size of the target. Only when max belly shrink"
+            " is 0, the\ncurrent belly is reduced by belly to lose. If both are"
+            " non-zero, only the max belly\nshrink is applied.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: belly to lose\nr3: max belly"
+            " shrink"
+        ),
+    )
+
+    TryIncreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restore belly and possibly boost max belly of the target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " belly to restore\nr3: max belly boost (if belly is full)\nstack[0]: flag"
+            " to log a message"
+        ),
+    )
+
+    TryInflictMuzzledStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Muzzled status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
     TryTransform = Symbol(
         None,
         None,
         None,
         (
             "Attempts to transform the target into the species of a random monster"
             " contained in the list returned by MonsterSpawnListPartialCopy.\n\nThe"
             " user pointer is only used when calling LogMessage functions.\n\nr0: user"
             " entity pointer\nr1: target entity pointer"
         ),
     )
 
+    TryInflictMobileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mobile status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictExposedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Exposed status condition on a target monster if possible."
+            " Only applies to\nGhost types and monsters with raised evasion. If the"
+            " animation effect ID is 0,\ndefaults to animation ID 0xE (this fallback"
+            " animation likely can't be seen in normal\nplay).\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: animation effect ID\nr3: flag to"
+            " only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryActivateIdentifyCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the flag for the identify orb which causes monsters holding items to"
+            " be shown with\na blue exclamation mark status icon.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictBlinkerStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Blinker status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting\nr3:"
+            " flag to log a message on failure\nreturn: Whether or not the status could"
+            " be inflicted"
+        ),
+    )
+
     IsBlinded = Symbol(
         [0x3B3D4],
         [0x2318CB4],
         None,
         (
             "Returns true if the monster has the blinded status (see"
             " statuses::blinded), or if it is not the leader and is holding Y-Ray"
             " Specs.\n\nr0: pointer to entity\nr1: flag for whether to check for the"
             " held item\nreturn: bool"
         ),
     )
 
+    TryInflictCrossEyedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Cross-Eyed status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEyedropStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Eyedrop status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSlipStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Slip status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nreturn: Whether or not"
+            " the status could be inflicted"
+        ),
+    )
+
+    TryInflictDropeyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Dropeye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
     RestoreMovePP = Symbol(
         [0x3B810],
         [0x23190F0],
         None,
         (
             "Restores the PP of all the target's moves by the specified amount.\n\nr0:"
             " user entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3:"
             " flag to suppress message logging"
         ),
     )
 
-    SetReflectDamageCountdownTo4 = Symbol(
+    ApplyProteinEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: attack boost"
+        ),
+    )
+
+    ApplyCalciumEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's special attack stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special attack boost"
+        ),
+    )
+
+    ApplyIronEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's defense stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: defense boost"
+        ),
+    )
+
+    ApplyZincEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's special defense stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special defense boost"
+        ),
+    )
+
+    TryInflictLongTossStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Long Toss status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictPierceStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Pierce status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictGastroAcidStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Gastro Acid status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    SetAquaRingHealingCountdownTo4 = Symbol(
         [0x3BFB0],
         [0x2319890],
         None,
         (
-            "Sets the monster's reflect damage countdown to a global value"
+            "Sets the countdown for Aqua Ring healing countdown to a global value"
             " (0x4).\n\nr0: pointer to entity"
         ),
     )
 
+    ApplyAquaRingHealing = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the passive healing gained from the Aqua Ring status.\n\nr0:"
+            " pointer to entity"
+        ),
+    )
+
+    TryInflictAquaRingStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Aqua Ring status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLuckyChantStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Lucky Chant status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictHealBlockStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Heal Block status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    MonsterHasEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the monster has the Embargo status condition.\n\nr0:"
+            " pointer to entity\nreturn: bool"
+        ),
+    )
+
+    LogItemBlockedByEmbargo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Logs the error message when the usage of an item is blocked by"
+            " Embargo.\n\nr0: pointer to entity"
+        ),
+    )
+
+    TryInflictEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Embargo status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictMiracleEyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Miracle Eye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting"
+        ),
+    )
+
+    TryInflictMagnetRiseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magnet Rise status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     HasConditionalGroundImmunity = Symbol(
         [0x3C63C],
         [0x2319F1C],
         None,
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    TryInflictSafeguardStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Safeguard status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMistStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mist status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWishStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Wish status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMagicCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magic Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLightScreenStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Light Screen status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictReflectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Reflect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Protect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictEndureStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Endure status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorMoveStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Move status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictConversion2Status = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Conversion2 status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictVitalThrowStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Vital Throw status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryResetStatChanges = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reset the stat changes of the defender.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr3: bool to force animation"
+        ),
+    )
+
     MirrorMoveIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
             " the effects is a status, 2 if it comes from an exclusive item, 0"
@@ -19019,21 +20455,101 @@
         (
             "Seems to apply an item's effect via a giant switch statement?\n\nr3:"
             " attacker pointer\nstack[0]: defender pointer\nstack[1]: thrown item"
             " pointer\nothers: ?"
         ),
     )
 
-    ViolentSeedBoost = Symbol(
+    ApplyCheriBerryEffect = Symbol(
         None,
         None,
         None,
         (
-            "Applies the Violent Seed boost to an entity.\n\nr0: attacker pointer\nr1:"
-            " defender pointer"
+            "Tries to heal the paralysis status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyPechaBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the poisoned and badly poisoned status condition. Prints a"
+            " message on\nfailure.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyRawstBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the burn status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyHungerSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Empties the targets belly to cause Hungry Pal status in non-leader"
+            " monsters and\nFamished in the leader monster.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyVileSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Reduces the targets defense and special defense stages to the lowest"
+            " level.\n\nr0: attacker pointer\nr1: defender pointer"
+        ),
+    )
+
+    ApplyViolentSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the target's offensive stats stages to the max.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGinsengEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the power of the move at the top of the target's Move List. Appears"
+            " to have a\nleftover check to boost the power of a move by 3 instead of 1"
+            " that always fails because\nthe chance is 0.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyBlastSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If thrown, unfreeze and deal fixed damage to the defender. If not thrown,"
+            " try to find \na monster in front of the attacker. If a monster is found"
+            " unfreeze and dedal fixed \ndamage to the defender. Appears to have a"
+            " leftover check for if the current fixed room is a boss fight and loads a"
+            " different pointer for the damage when used in a boss room.\nHowever, this"
+            " isn't noticeable because both the normal and boss damage is the"
+            " same.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: bool"
+            " thrown"
         ),
     )
 
     ApplyGummiBoostsDungeonMode = Symbol(
         [0x40CA8],
         [0x231E588],
         None,
@@ -19075,14 +20591,68 @@
         None,
         (
             "If the target monster is a Linoone, restores all the PP of all the"
             " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
+    ApplyDoughSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a team member, set dough_seed_extra_poke_flag to"
+            " true to \nmake extra poke spawn on the next floor. Otherwise, do"
+            " nothing.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyViaSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to randomly teleport the target with a message for eating the"
+            " seed.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGravelyrockEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restores 10 hunger to the target and will raise the target's IQ if they"
+            " are a bonsly\nor sudowoodo.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyGonePebbleEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Causes a few visual effects, temporarily changes the dungeon music to the"
+            " Goodnight\ntrack, and gives the target the enduring status.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGracideaEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target is Shaymin, attempt to change the target's form to Shaymin"
+            " Sky Forme. Otherwise, do nothing.\n\nr0: user entity pointer\nr1: target"
+            " entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -19156,15 +20726,29 @@
         None,
         None,
         None,
         (
             "Creates an explosion if possible.\n\nThe target monster is considered the"
             " source of the explosion.\n\nr0: user entity pointer\nr1: target entity"
             " pointer\nr2: coordinates where the explosion should take place"
-            " (unverified)\nr3: ?\nstack[0]: ?\nstack[1]: damage source (normally"
+            " (center)\nr3: explosion radius (only works correctly with 1 and"
+            " 2)\nstack[0]: damage type\nstack[1]: damage source"
+        ),
+    )
+
+    TryAftermathExplosion = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Creates the explosion for the ability aftermath if possible.\n\nThe target"
+            " monster is considered the source of the explosion.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: coordinates where the explosion"
+            " should take place (center)\nr3: explosion radius (only works correctly"
+            " with 1 and 2)\nstack[0]: damage type\nstack[1]: damage source (normally"
             " DAMAGE_SOURCE_EXPLOSION)"
         ),
     )
 
     TryWarp = Symbol(
         [0x448D4],
         [0x23221B4],
@@ -19638,14 +21222,57 @@
     GetStairsRoom = Symbol(
         [0x59F18],
         [0x23377F8],
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    UpdateTrapsVisibility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Exact purpose unknown. Gets called whenever a trap tile is shown or"
+            " hidden.\n\nNo params."
+        ),
+    )
+
+    DrawTileGrid = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Draws a grid on the nearby walkable tiles. Triggered by pressing Y.\n\nr0:"
+            " Coordinates of the entity around which the grid will be drawn\nr1: ?\nr2:"
+            " ?\nr3: ?"
+        ),
+    )
+
+    HideTileGrid = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Hides the grid on the nearby walkable tiles. Triggered by releasing"
+            " Y.\n\nNo params."
+        ),
+    )
+
+    DiscoverMinimap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Discovers the tiles around the specified position on the minimap.\n\nThe"
+            " discovery radius depends on the visibility range of the floor. If"
+            " display_data::blinded is true, the function returns early without doing"
+            " anything.\n\nr0: Position around which the map should be discovered"
+        ),
+    )
+
     IsWaterTileset = Symbol(
         None,
         None,
         None,
         (
             "Returns flag tileset_property::is_water_tileset for the current"
             " tileset\n\nreturn: True if the current tileset is a water tileset"
@@ -19711,14 +21338,34 @@
         (
             "Sets the boost_kecleon_shop_spawn_chance field on the dungeon struct"
             " depending on if a team member has the exclusive item effect for more"
             " kecleon shops.\n\nNo params."
         ),
     )
 
+    SetDoughSeedFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the dough_seed_extra_money_flag field on the dungeon struct to the"
+            " given value.\n\nr0: bool to set the flag to"
+        ),
+    )
+
+    TrySpawnDoughSeedPoke = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the dough_seed_extra_money_flag field on the dungeon struct and"
+            " tries to spawn\nextra poke if it is set.\n\nNo params."
+        ),
+    )
+
     IsSecretBazaar = Symbol(
         None,
         None,
         None,
         "Checks if the current floor is the Secret Bazaar.\n\nreturn: bool",
     )
 
@@ -19769,28 +21416,62 @@
         None,
         (
             "Checks if the current floor is a secret bazaar or a secret"
             " room.\n\nreturn: bool"
         ),
     )
 
+    HiddenStairsPresent = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the hidden stairs are present on this floor.\n\nThe function"
+            " checks that dungeon_generation_info::hidden_stairs_pos isn't (-1,"
+            " -1)\n\nreturn: True if the hidden stairs are present on this floor, false"
+            " otherwise."
+        ),
+    )
+
+    HiddenStairsTrigger = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called whenever the leader steps on the hidden stairs.\n\nIf the stairs"
+            " hadn't been revealed yet, plays the corresponding animation.\n\nr0: True"
+            " to display a message if the stairs are revealed, false to omit it."
+        ),
+    )
+
     GetDungeonGenInfoUnk0C = Symbol(
         None, None, None, "return: dungeon_generation_info::field_0xc"
     )
 
     GetMinimapData = Symbol(
         None,
         None,
         None,
         (
             "Returns a pointer to the minimap_display_data struct in the dungeon"
             " struct.\n\nreturn: minimap_display_data*"
         ),
     )
 
+    DrawMinimapTile = Symbol(
+        None,
+        None,
+        None,
+        "Draws a single tile on the minimap.\n\nr0: X position\nr1: Y position",
+    )
+
+    UpdateMinimap = Symbol(
+        None, None, None, "Graphically updates the minimap\n\nNo params."
+    )
+
     SetMinimapDataE447 = Symbol(
         [0x5DCFC],
         [0x233B5DC],
         None,
         (
             "Sets minimap_display_data::field_0xE447 to the specified value\n\nr0:"
             " Value to set the field to"
@@ -19814,14 +21495,35 @@
         None,
         (
             "Sets minimap_display_data::field_0xE448 to the specified value\n\nr0:"
             " Value to set the field to"
         ),
     )
 
+    InitWeirdMinimapMatrix = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the matrix at minimap_display_data+0xE000. Seems to overflow"
+            " said matrix when doing so.\n\nNo params."
+        ),
+    )
+
+    InitMinimapDisplayTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to initialize an instance of struct minimap_display_tile\n\nr0:"
+            " Pointer to struct to init\nr1: Seems to be a pointer to the file that"
+            " stores minimap icons or something like that"
+        ),
+    )
+
     LoadFixedRoomDataVeneer = Symbol(
         None,
         None,
         None,
         (
             "Likely a linker-generated veneer for LoadFixedRoomData.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nNo"
@@ -20513,14 +22215,24 @@
             " reached by the traversal algorithm, then the stairs must not be reachable"
             " from that tile.\n\nr0: x coordinate of the stairs\nr1: y coordinate of"
             " the stairs\nr2: flag to always return true, but set a special bit on all"
             " walkable tiles that aren't reachable from the stairs\nreturn: bool"
         ),
     )
 
+    GetNextFixedRoomAction = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the next action that needs to be performed when spawning a fixed"
+            " room tile.\n\nreturn: Next action ID"
+        ),
+    )
+
     ConvertWallsToChasms = Symbol(
         [0x66028], [0x2343908], None, "Converts all wall tiles to chasms.\n\nNo params."
     )
 
     ResetInnerBoundaryTileRows = Symbol(
         [0x6665C],
         [0x2343F3C],
@@ -20571,25 +22283,75 @@
             " HIDDEN_STAIRS_RANDOM_SECRET_BAZAAR_OR_SECRET_ROOM and the"
             " floor_properties::hidden_stairs_spawn_chance) into a concrete hidden"
             " stairs type.\n\nr0: dungeon generation info pointer\nr1: floor properties"
             " pointer\nreturn: enum hidden_stairs_type"
         ),
     )
 
+    GetFinalKecleonShopSpawnChance = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the kecleon shop spawn chance for the floor.\n\nWhen"
+            " dungeon::boost_kecleon_shop_spawn_chance is false, returns the same value"
+            " as the input. When it's true, returns the input (chance * 1.2).\n\nr0:"
+            " base kecleon shop spawn chance,"
+            " floor_properties::kecleon_shop_spawn_chance\nreturn: int"
+        ),
+    )
+
     ResetHiddenStairsSpawn = Symbol(
         [0x669EC],
         [0x23442CC],
         None,
         (
             "Resets hidden stairs spawn information for the floor. This includes the"
             " position on the floor generation status as well as the flag indicating"
             " whether the spawn was blocked.\n\nNo params."
         ),
     )
 
+    PlaceFixedRoomTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to spawn a single tile when generating a fixed room. The tile might"
+            " contain an item or a monster.\n\nr0: Pointer to the tile to spawn\nr1:"
+            " Fixed room action to perform. Controls what exactly will be spawned. The"
+            " action is actually 12 bits long, the highest 4 bits are used as a"
+            " parameter that represents a direction (for example, when spawning a"
+            " monster).\nr2: Tile X position\nr3: Tile Y position"
+        ),
+    )
+
+    FixedRoomActionParamToDirection = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Converts the parameter stored in a fixed room action value to a direction"
+            " ID.\n\nThe conversion is performed by subtracting 1 to the value. If the"
+            " parameter had a value of 0, DIR_NONE is returned.\n\nr0: Parameter"
+            " value\nreturn: Direction"
+        ),
+    )
+
+    ApplyKeyEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to open a locked door in front of the target if a locked door has"
+            " not already\nbeen open on the floor.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
     LoadFixedRoomData = Symbol(
         [0x67874],
         [0x2345154],
         None,
         (
             "Loads fixed room data from BALANCE/fixed.bin into the buffer pointed to by"
             " FIXED_ROOM_DATA_PTR.\n\nNo params."
@@ -21372,15 +23134,25 @@
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
             " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
-        [0x717A0], [0x234F080], None, "Note: unverified, ported from Irdkwia's notes"
+        [0x717A0],
+        [0x234F080],
+        None,
+        (
+            "Opens a menu. The menu to open depends on the specified parameter.\n\nIt"
+            " looks like the function takes a parameter in r0, but doesn't use it. r1"
+            " doesn't even get set when this function is called.\n\nr0: (?) Unused by"
+            " the function. Seems to be 1 byte long.\nr1: (?) Unused by the function."
+            " Seems to be 1 byte long.\nr2: True to open the bag menu, false to open"
+            " the main dungeon menu"
+        ),
     )
 
     OthersMenuLoop = Symbol(
         [0x73160],
         [0x2350A40],
         None,
         (
@@ -21556,27 +23328,27 @@
         None,
         (
             "The move target and range code for special healing moves that target just"
             " the user (0x273).\n\ntype: struct move_target_and_range (+ padding)"
         ),
     )
 
-    PLAIN_SEED_VALUE = Symbol(
-        None, None, None, "Some value related to the Plain Seed (0xBE9)."
+    PLAIN_SEED_STRING_ID = Symbol(
+        None, None, None, "The string ID for eating a Plain Seed (0xBE9)."
     )
 
     MAX_ELIXIR_PP_RESTORATION = Symbol(
         None,
         None,
         None,
         "The amount of PP restored per move by ingesting a Max Elixir (0x3E7).",
     )
 
-    SLIP_SEED_VALUE = Symbol(
-        None, None, None, "Some value related to the Slip Seed (0xC75)."
+    SLIP_SEED_FAIL_STRING_ID = Symbol(
+        None, None, None, "The string ID for when eating the Slip Seed fails (0xC75)."
     )
 
     ROCK_WRECKER_MOVE_ID = Symbol(
         None, None, None, "The move ID for Rock Wrecker (453)."
     )
 
     CASTFORM_NORMAL_FORM_MALE_ID = Symbol(
@@ -22321,15 +24093,28 @@
     loadaddress = 0x233E300
     length = 0xA160
     functions = JpOverlay3Functions
     data = JpOverlay3Data
 
 
 class JpOverlay30Functions:
-    pass
+    WriteQuicksaveData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Function responsible for writing dungeon data when quicksaving.\n\nAmong"
+            " other things, it contains a loop that goes through all the monsters in"
+            " the current dungeon, copying their data to the buffer. The data is not"
+            " copied as-is though, the game uses a reduced version of the monster"
+            " struct containing only the minimum required data to resume the game"
+            " later.\n\nr0: Pointer to buffer where data should be written\nr1: Buffer"
+            " size. Seems to be 0x5800 (22 KB) when the function is called."
+        ),
+    )
 
 
 class JpOverlay30Data:
     OVERLAY30_JP_STRING_1 = Symbol([0x3840], [0x23872E0], 0xC, "みさき様")
 
     OVERLAY30_JP_STRING_2 = Symbol([0x384C], [0x23872EC], 0xC, "やよい様")
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -1020,17 +1020,17 @@
 
     LoadFileInPackWithPackId = Symbol(
         None,
         None,
         None,
         (
             "Call LoadFileInPack after looking up the global Pack archive by its"
-            " identifier\n\nr0: pack file identifier\nr1: [output] target buffer\nr2:"
-            " file index\nreturn: number of read bytes (identical to the length of the"
-            " pack from the Table of Content)"
+            " identifier\n\nr0: pack file identifier\nr1: file index\nr2: [output]"
+            " target buffer\nreturn: number of read bytes (identical to the length of"
+            " the pack from the Table of Content)"
         ),
     )
 
     AllocAndLoadFileInPack = Symbol(
         None,
         None,
         None,
@@ -1071,14 +1071,27 @@
             "Load the indexed file from the Pack archive, itself loaded from the"
             " ROM.\n\nr0: pack file struct\nr1: [output] target buffer\nr2: file"
             " index\nreturn: number of read bytes (identical to the length of the pack"
             " from the Table of Content)"
         ),
     )
 
+    GetDungeonResultMsg = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the message that is shown on the dungeon results ('The Last Outing')"
+            " screen, right after the leader's name.\n\nr0: Damage source value to use"
+            " when displaying the cause of fainting or the result of the"
+            " expedition\nr1: [output] Buffer where the resulting message will be"
+            " stored\nr2: Buffer size\nr3: (?) Seems to point to a buffer"
+        ),
+    )
+
     GetDamageSource = Symbol(
         None,
         None,
         None,
         (
             "Gets the damage source for a given move-item combination.\n\nIf there's no"
             " item, the source is the move ID. If the item is an orb, return"
@@ -1153,14 +1166,26 @@
         None,
         (
             "Checks if an item is one of the aura bows received at the start of the"
             " game.\n\nr0: item ID\nreturn: bool"
         ),
     )
 
+    IsTreasureBox = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the given item ID is a treasure box\n\nIn particular, it checks"
+            " if the category of the item is CATEGORY_TREASURE_BOXES_1,"
+            " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
+            " ID\nreturn: True if the item is a treasure box, false otherwise"
+        ),
+    )
+
     InitItem = Symbol(
         None,
         None,
         None,
         (
             "Initialize an item struct with the given information.\n\nThis will resolve"
             " the quantity based on the item type. For Poké, the quantity code will"
@@ -1441,22 +1466,21 @@
     GetItemMoveId = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: move ID",
     )
 
-    TestItemFlag0xE = Symbol(
+    TestItemAiFlag = Symbol(
         None,
         None,
         None,
         (
-            "Tests bit 7 if r1 is 0, bit 6 if r1 is 1, bit 5 otherwise\n\nNote:"
-            " unverified, ported from Irdkwia's notes\n\nr0: item ID\nr1:"
-            " bit_id\nreturn: bool"
+            "Used to check the AI flags for an item. Tests bit 7 if r1 is 0, bit 6 if"
+            " r1 is 1, bit\n5 otherwise.\n\nr0: item ID\nr1: bit_id\nreturn: bool"
         ),
     )
 
     IsItemInTimeDarkness = Symbol(
         None,
         None,
         None,
@@ -1494,14 +1518,25 @@
         None,
         (
             "Sets the amount of money the player is carrying, clamping the value to the"
             " range [0, MAX_MONEY_CARRIED].\n\nr0: new value"
         ),
     )
 
+    AddMoneyCarried = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds the amount of money to the player's current amount of money. Just"
+            " calls\nSetMoneyCarried with the current money + money gained.\n\nr0:"
+            " money gained (can be negative)"
+        ),
+    )
+
     GetCurrentBagCapacity = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: bag capacity",
     )
 
@@ -1522,15 +1557,18 @@
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: # items",
     )
 
     CountNbItemsOfTypeInBag = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: count",
+        (
+            "Returns the number of items of the given kind in the bag\n\nr0: item"
+            " ID\nreturn: count"
+        ),
     )
 
     CountItemTypeInBag = Symbol(
         None,
         None,
         None,
         (
@@ -1742,14 +1780,24 @@
     ScriptSpecialProcess0x39 = Symbol(
         None,
         None,
         None,
         "Implements SPECIAL_PROC_0x39 (see ScriptSpecialProcessCall).\n\nreturn: bool",
     )
 
+    CountNbItemsOfTypeInStorage = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the number of items of the given kind in the storage\n\nr0: item"
+            " ID\nreturn: count"
+        ),
+    )
+
     CountItemTypeInStorage = Symbol(
         None,
         None,
         None,
         (
             "Implements SPECIAL_PROC_COUNT_ITEM_TYPE_IN_STORAGE (see"
             " ScriptSpecialProcessCall).\n\nr0: pointer to an owned_item\nreturn:"
@@ -2588,38 +2636,62 @@
     StopSe = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
 
     DeleteWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
+            "Always delete an entry if the file is allocated externally"
+            " (file_externally_allocated is set), otherwise, decrease the reference"
+            " counter. If it reach 0, delete the sprite.\n\nr0: wan_table_ptr\nr1:"
             " wan_id"
         ),
     )
 
+    AllocateWanTableEntry = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return the identifier to a free wan table entry (-1 if none are"
+            " avalaible). The entry is zeroed.\n\nr0: wan_table_ptr\nreturn: the entry"
+            " id in wan_table"
+        ),
+    )
+
     FindWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Appears to search in the given table (in practice always seems to be"
+            "Search in the given table (in practice always seems to be"
             " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
             " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
             " if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "wan_id = -1 if it is not loaded\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: wan_table_ptr\nr1: bin_file_id\nr2: file_id\nreturn: wan_id"
+            "Look up a sprite with the provided pack_id and file_index in the wan"
+            " table.\n\nr0: wan_table_ptr\nr1: pack_id\nr2: file_index\nreturn: sprite"
+            " id in the wan table, -1 if not found"
+        ),
+    )
+
+    InitWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the input WAN table with 0x60 free entries (it needs a length"
+            " of 0x1510 bytes)\n\nr0: wan_table_ptr"
         ),
     )
 
     LoadWanTableEntry = Symbol(
         None,
         None,
         None,
@@ -2627,14 +2699,40 @@
             "Appears to load data from the given file (in practice always seems to be"
             " animation data), using previously loaded data in the given table (see"
             " FindWanTableEntry) if possible.\n\nr0: table pointer\nr1: file name\nr2:"
             " flags\nreturn: table index of the loaded data"
         ),
     )
 
+    LoadWanTableEntryFromPack = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3: allocation"
+            " flags\nstack[0]: compressed\nreturn: the entry id in wan_table"
+        ),
+    )
+
+    LoadWanTableEntryFromPackUseProvidedMemory = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite into the"
+            " provided memory area. Mark the sprite as externally allocated.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3:"
+            " sprite_storage_ptr\nstack[0]: compressed\nreturn: the entry id in"
+            " wan_table"
+        ),
+    )
+
     ReplaceWanFromBinFile = Symbol(
         None,
         None,
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
             " wan_id\nr2: bin_file_id\nr3: file_id\nstack[0]: compressed"
@@ -2890,14 +2988,30 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetStringPower = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    GetDungeonResultString = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns a string containing some information to be used when displaying"
+            " the dungeon results screen.\n\nThe exact string returned depends on the"
+            " value of r0:\n0: Name of the move that fainted the leader. Empty string"
+            " if the leader didn't faint.\n1-3: Seems to always result in an empty"
+            " string.\n4: Name of the pokémon that fainted the leader, or name of the"
+            " leader if the leader didn't faint.\n5: Name of the fainted leader. Empty"
+            " string if the leader didn't faint.\n\nr0: String to return\nreturn:"
+            " Pointer to resulting string"
+        ),
+    )
+
     SetQuestionMarks = Symbol(
         None,
         None,
         None,
         (
             "Fills the buffer with the string '???'\n\nNote: unverified, ported from"
             " Irdkwia's notes\n\nr0: buffer"
@@ -3196,15 +3310,15 @@
 
     IsMenuOptionActive = Symbol(
         None,
         None,
         None,
         (
             "Called whenever a menu option is selected. Returns whether the option is"
-            " active or not.\n\nr0: ?\nReturn: True if the menu option is enabled,"
+            " active or not.\n\nr0: ?\nreturn: True if the menu option is enabled,"
             " false otherwise."
         ),
     )
 
     ShowKeyboard = Symbol(
         None,
         None,
@@ -3570,14 +3684,24 @@
         None,
         (
             "Gets the special episode type from the SPECIAL_EPISODE_TYPE script"
             " variable.\n\nreturn: special episode type"
         ),
     )
 
+    GetExecuteSpecialEpisodeType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the special episode type from the EXECUTE_SPECIAL_EPISODE_TYPE script"
+            " variable.\n\nreturn: special episode type"
+        ),
+    )
+
     HasPlayedOldGame = Symbol(
         None,
         None,
         None,
         "Returns the value of the VAR_PLAY_OLD_GAME script variable.\n\nreturn: bool",
     )
 
@@ -3640,21 +3764,21 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: dungeon ID\nr1:"
             " bit_value"
         ),
     )
 
-    CheckDungeonOpen = Symbol(
+    GetDungeonMode = Symbol(
         None,
         None,
         None,
         (
-            "Related to dungeon open list\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: dungeon ID\nreturn: status code?"
+            "Returns the mode of the specified dungeon\n\nr0: Dungeon ID\nreturn:"
+            " Dungeon mode"
         ),
     )
 
     GlobalProgressAlloc = Symbol(
         None,
         None,
         None,
@@ -3861,14 +3985,59 @@
         (
             "If buffer_portrait is null, it only checks if it exists\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: portrait box pointer\nr1:"
             " buffer_portrait\nreturn: exists"
         ),
     )
 
+    SetEnterDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to set the dungeon that will be accessed when switching from ground"
+            " to dungeon mode.\n\nr0: Dungeon ID"
+        ),
+    )
+
+    InitDungeonInit = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the dungeon_init struct before entering a dungeon.\n\nr0:"
+            " [output] Pointer to the struct to init\nr1: Dungeon ID"
+        ),
+    )
+
+    IsNoLossPenaltyDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the specified dungeon shouldn't have a loss penalty.\n\nIf"
+            " true you won't lose your money and items upon fainting. Also used to"
+            " initialize dungeon_init::skip_faint_animation_flag.\n\nReturns: True for"
+            " DUNGEON_CRYSTAL_LAKE and DUNGEON_5TH_STATION_CLEARING, as well as for"
+            " DUNGEON_DEEP_STAR_CAVE_TEAM_ROGUE if the ground variable SIDE01_BOSS2ND"
+            " is 0; false otherwise."
+        ),
+    )
+
+    CheckMissionRestrictions = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Seems to be used to check if you have any missions that have unmet"
+            " restrictions when trying to access a dungeon.\n\nr0: ?\nreturn: (?) Seems"
+            " to be composed of multiple bitflags."
+        ),
+    )
+
     GetNbFloors = Symbol(
         None,
         None,
         None,
         (
             "Returns the number of floors of the given dungeon.\n\nThe result is"
             " hardcoded for certain dungeons, such as dojo mazes.\n\nr0: Dungeon"
@@ -3930,19 +4099,75 @@
         (
             "Given a dungeon ID and a floor number, returns a struct with the"
             " corresponding dungeon group and floor number in that group.\n\nThe"
             " function normally uses the data in mappa_s.bin to calculate the result,"
             " but there's some dungeons (such as dojo mazes) that have hardcoded return"
             " values.\n\nIrdkwia's notes:\n  [r1]: dungeon_id\n  [r1+1]:"
             " dungeon_floor_id\n  [r0]: group_id\n  [r0+1]: group_floor_id\n\nr0:"
-            " (output) Struct containing the dungeon group and floor group\nr1: Struct"
+            " [output] Struct containing the dungeon group and floor group\nr1: Struct"
             " containing the dungeon ID and floor number"
         ),
     )
 
+    GetMissionRank = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the mission rank for the given dungeon and floor.\n\nIf the dungeon"
+            " ID is >= DUNGEON_NORMAL_FLY_MAZE or the group of the dungeon is >"
+            " DGROUP_DUMMY_0x63, returns MISSION_RANK_E.\n\nr0: Dungeon and"
+            " floor\nreturn: Mission rank"
+        ),
+    )
+
+    GetOutlawLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for outlaws for the given dungeon and"
+            " floor\n\nr0: Dungeon and floor\nreturn: Outlaw level"
+        ),
+    )
+
+    GetOutlawLeaderLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for team leader outlaws for the given"
+            " dungeon and floor. Identical to GetOutlawLevel.\n\nr0: Dungeon and"
+            " floor\nreturn: Outlaw leader level"
+        ),
+    )
+
+    GetOutlawMinionLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for minion outlaws for the given"
+            " dungeon and floor.\n\nr0: Dungeon and floor\nreturn: Outlaw minion level"
+        ),
+    )
+
+    AddGuestMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds a guest monster to the active team\n\nr0: dungeon_init struct for the"
+            " dungeon that is about to be entered\nr1: Number of the guest monster to"
+            " add. Used when more than one monster is added.\nr2: Pointer to the guest"
+            " monster entry to add to the team (usually located within"
+            " GUEST_MONSTER_DATA)"
+        ),
+    )
+
     GetGroundNameId = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetAdventureLogStructLocation = Symbol(
         None,
         None,
@@ -5010,14 +5235,24 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: family index",
     )
 
     LoadM2nAndN2m = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    GuestMonsterToGroundMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inits a ground_monster entry with the given guest_monster struct.\n\nr0:"
+            " [output] ground_monster struct to init\nr1: guest_monster struct to use"
+        ),
+    )
+
     StrcmpMonsterName = Symbol(
         None,
         None,
         None,
         (
             "Checks if the string_buffer matches the name of the species\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: string_buffer\nr1: monster"
@@ -5586,15 +5821,15 @@
         None,
         None,
         None,
         (
             "Determines the list of IQ skills that a given monster can learn given its"
             " IQ value.\n\nThe list of skills is written in the array specified in r0."
             " The array has 69 slots in total. Unused slots are set to 0.\n\nr0:"
-            " (output) Array where the list of skills will be written\nr1: Monster"
+            " [output] Array where the list of skills will be written\nr1: Monster"
             " species\nr2: Monster IQ\nreturn: Amount of skills written to the output"
             " array"
         ),
     )
 
     DisableIqSkill = Symbol(
         None,
@@ -6023,26 +6258,121 @@
         (
             "Converts an index in DUNGEON_SWAP_ID_TABLE to the corresponding dungeon"
             " ID, or DUNGEON_DUMMY_0xFF if the index is -1.\n\nr0: index\nreturn:"
             " dungeon ID"
         ),
     )
 
+    GetDungeonModeSpecial = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the status of the given dungeon, with some modifications.\n\nIf"
+            " the dungeon ID is DUNGEON_BEACH, returns DMODE_REQUEST.\nIf it's"
+            " DUNGEON_JOINED_AT_UNKNOWN, returns DMODE_OPEN_AND_REQUEST.\nIf it's >="
+            " DUNGEON_NORMAL_FLY_MAZE and <= DUNGEON_DOJO_0xD3, returns"
+            " DMODE_OPEN_AND_REQUEST.\nElse, calls GetDungeonMode and returns"
+            " DMODE_REQUEST if the dungeon has been cleared, or DMODE_OPEN if it's"
+            " not.\n\nr0: Dungeon ID\nreturn: Dungeon mode"
+        ),
+    )
+
     ResumeBgm = Symbol(
         None, None, None, "Uncertain.\n\nNote: unverified, ported from Irdkwia's notes"
     )
 
     FlushChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     UpdateChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    ClearIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enables processor interrupts by clearing the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were disabled, 0x0 if they were already enabled)"
+        ),
+    )
+
+    EnableIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Disables processor interrupts by setting the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were already disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    SetIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the value of the processor's interrupt flag according to the"
+            " specified parameter.\n\nr0: Value to set the flag to (0x80 to set it,"
+            " which disables interrupts; 0x0 to unset it, which enables"
+            " interrupts)\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts were"
+            " disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    EnableIrqFiqFlags = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Disables processor all interrupts (both standard and fast) by setting the"
+            " i and f flags in the program status register (cpsr).\n\nreturn: Old value"
+            " of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    SetIrqFiqFlags = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the value of the processor's interrupt flags (i and f) according to"
+            " the specified parameter.\n\nr0: Value to set the flags to (0xC0 to set"
+            " both flags, 0x80 to set the i flag and clear the f flag, 0x40 to set the"
+            " f flag and clear the i flag and 0x0 to clear both flags)\nreturn: Old"
+            " value of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    GetIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the current value of the processor's interrupt request (i)"
+            " flag\n\nreturn: cpsr & 0x80 (0x80 if interrupts are disabled, 0x0 if they"
+            " are enabled)"
+        ),
+    )
+
+    WaitForever2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EnableIrqFlag and WaitForInterrupt in an infinite loop.\n\nThis is"
+            " called on fatal errors to hang the program indefinitely.\n\nNo params."
+        ),
+    )
+
     WaitForInterrupt = Symbol(
         None,
         None,
         None,
         (
             "Presumably blocks until the program receives an interrupt.\n\nThis just"
             " calls (in Ghidra terminology) coproc_moveto_Wait_for_interrupt(0). See"
@@ -12617,14 +12947,24 @@
         None,
         (
             "The multiplier for damage from the Air Blade (1.5), as a binary"
             " fixed-point number (8 fraction bits)"
         ),
     )
 
+    KECLEON_SHOP_BOOST_CHANCE_MULTIPLIER = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The boosted kecleon shop spawn chance multiplier (~1.2) as a binary"
+            " fixed-point number (8 fraction bits)."
+        ),
+    )
+
     HIDDEN_STAIRS_SPAWN_CHANCE_MULTIPLIER = Symbol(
         None,
         None,
         None,
         (
             "The hidden stairs spawn chance multiplier (~1.2) as a binary fixed-point"
             " number (8 fraction bits), if applicable. See"
@@ -13301,16 +13641,18 @@
     )
 
     LoadBackgroundAttributes = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: [output]"
-            " bg_attr_str\nr1: bg_id"
+            "Open and read an entry from the MAP_BG/bg_list.dat\n\nDocumentation on"
+            " this format can be found"
+            " here:\nhttps://github.com/SkyTemple/skytemple-files/tree/55b3017631a8a1b0f106111ef91a901dc394c6df/skytemple_files/graphics/bg_list_dat\n\nr0:"
+            " [output] The entry\nr1: background ID"
         ),
     )
 
     LoadMapType10 = Symbol(
         None,
         None,
         None,
@@ -13413,14 +13755,24 @@
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
             " characters printed, excluding the null-terminator"
         ),
     )
 
+    GetExclusiveItemRequirements = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to calculate the items required to get a certain exclusive item in"
+            " the swap shop.\n\nr0: ?\nr1: ?"
+        ),
+    )
+
     StatusUpdate = Symbol(
         None,
         None,
         None,
         (
             "Implements SPECIAL_PROC_STATUS_UPDATE (see"
             " ScriptSpecialProcessCall).\n\nNo params."
@@ -13579,14 +13931,18 @@
         ),
     )
 
     UNIONALL_RAM_ADDRESS = Symbol(None, None, None, "[Runtime]")
 
     GROUND_STATE_MAP = Symbol(None, None, None, "[Runtime]")
 
+    GROUND_STATE_WEATHER = Symbol(
+        None, None, None, "[Runtime] Same structure format as GROUND_STATE_MAP"
+    )
+
     GROUND_STATE_PTRS = Symbol(
         None,
         None,
         None,
         (
             "Host pointers to multiple structure used for performing an overworld"
             " scene\n\ntype: struct main_ground_data"
@@ -15430,24 +15786,81 @@
     FadeToBlack = Symbol(
         None,
         None,
         None,
         "Fades the screen to black across several frames.\n\nNo params.",
     )
 
+    CheckTouchscreenArea = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the currently pressed touchscreen position is within the"
+            " specified area.\n\nr0: Area lower X coordinate\nr1: Area lower Y"
+            " coordinate\nr2: Area upper X coordinate\nr3: Area upper Y"
+            " coordinate\nreturn: True if the specified area contains the currently"
+            " pressed touchscreen position, false otherwise."
+        ),
+    )
+
+    GetTrapInfo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Given a trap entity, returns the pointer to the trap info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Trap data pointer"
+        ),
+    )
+
+    GetItemInfo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Given an item entity, returns the pointer to the item info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Item data pointer"
+        ),
+    )
+
     GetTileAtEntity = Symbol(
         None,
         None,
         None,
         (
             "Returns a pointer to the tile where an entity is located.\n\nr0: pointer"
             " to entity\nreturns: pointer to tile"
         ),
     )
 
+    UpdateEntityPixelPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Updates an entity's pixel_pos field using the specified pixel_position"
+            " struct, or its own pos field if it's null.\n\nr0: Entity pointer\nr1:"
+            " Pixel position to use, or null to use the entity's own position"
+        ),
+    )
+
+    CreateEnemyEntity = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Creates and initializes the entity struct of a newly spawned enemy"
+            " monster. Fails if there's 16 enemies on the floor already.\n\nIt could"
+            " also be used to spawn fixed room allies, since those share their slots on"
+            " the entity list.\n\nr0: Monster ID\nreturn: Pointer to the newly"
+            " initialized entity, or null if the entity couldn't be initialized"
+        ),
+    )
+
     SpawnTrap = Symbol(
         None,
         None,
         None,
         (
             "Spawns a trap on the floor. Fails if there are more than 64 traps already"
             " on the floor.\n\nThis modifies the appropriate fields on the dungeon"
@@ -15467,35 +15880,46 @@
             " items already on the floor.\n\nThis initializes a new entry in the entity"
             " table and points it to the corresponding slot in the item info"
             " list.\n\nr0: position\nreturn: entity pointer for the newly added item,"
             " or null on failure"
         ),
     )
 
-    ShouldDisplayEntityMessages = Symbol(
+    ShouldMinimapDisplayEntity = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if a given entity should be displayed on the minimap\n\nr0: Entity"
+            " pointer\nreturn: True if the entity should be displayed on the minimap"
+        ),
+    )
+
+    ShouldDisplayEntity = Symbol(
         None,
         None,
         None,
         (
-            "Checks if messages that involve a certain entity should be displayed or"
-            " suppressed.\n\nFor example, it returns false if the entity is an"
-            " invisible enemy.\n\nr0: Entity pointer\nr1: ?\nreturn: True if messages"
-            " involving the entity should be displayed, false if they should be"
-            " suppressed."
+            "Checks if an entity should be displayed or not.\n\nFor example, it returns"
+            " false if the entity is an invisible enemy.\nAlso used to determine if"
+            " messages that involve a certain entity should be displayed or"
+            " suppressed.\n\nr0: Entity pointer\nr1: (?) Seems to be 1 for monsters and"
+            " 0 for items.\nreturn: True if the entity and its associated messages"
+            " should be displayed, false if they shouldn't."
         ),
     )
 
-    ShouldDisplayEntityMessagesWrapper = Symbol(
+    ShouldDisplayEntityWrapper = Symbol(
         None,
         None,
         None,
         (
-            "Calls ShouldDisplayEntityMessages with r1 = 0\n\nr0: Entity"
-            " pointer\nreturn: True if messages involving the entity should be"
-            " displayed, false if they should be suppressed."
+            "Calls ShouldDisplayEntity with r1 = 0\n\nr0: Entity pointer\nreturn: True"
+            " if the entity and its associated messages should be displayed, false if"
+            " they shouldn't."
         ),
     )
 
     CanSeeTarget = Symbol(
         None,
         None,
         None,
@@ -15615,28 +16039,54 @@
         (
             "Returns dungeon::display_data::visibility_range. If the visibility range"
             " is 0, returns 2 instead.\n\nreturn: Visibility range of the current"
             " floor, or 2 if the visibility is 0."
         ),
     )
 
-    PlayEffectAnimation = Symbol(
+    PlayEffectAnimationEntity = Symbol(
         None,
         None,
         None,
         (
             "Just a guess. This appears to be paired often with"
             " GetEffectAnimationField0x19, and also has calls AnimationHasMoreFrames in"
             " a loop alongside AdvanceFrame(66) calls.\n\nThe third parameter skips the"
             " loop entirely. It seems like in this case the function might just preload"
-            " some animation frames for later use??\n\nr0: entity pointer\nr1: ?\nr2:"
-            " appears to be a flag for actually running the animation now? If this is"
-            " 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn: status"
-            " code, or maybe the number of frames or something? Either way, -1 seems to"
-            " indicate the animation being finished or something?"
+            " some animation frames for later use??\n\nr0: entity pointer\nr1: Effect"
+            " ID\nr2: appears to be a flag for actually running the animation now? If"
+            " this is 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn:"
+            " status code, or maybe the number of frames or something? Either way, -1"
+            " seems to indicate the animation being finished or something?"
+        ),
+    )
+
+    PlayEffectAnimationPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Takes a position struct in r0 and converts it to a pixel position struct"
+            " before calling PlayEffectAnimationPixelPos\n\nr0: Position where the"
+            " effect should be played\nr1: Effect ID\nr2: Unknown flag (same as the one"
+            " in PlayEffectAnimationEntity)\nreturn: Result of call to"
+            " PlayEffectAnimationPixelPos"
+        ),
+    )
+
+    PlayEffectAnimationPixelPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Seems like a variant of PlayEffectAnimationEntity that uses pixel"
+            " coordinates as its first parameter instead of an entity pointer.\n\nr0:"
+            " Pixel position where the effect should be played\nr1: Effect ID\nr2:"
+            " Unknown flag (same as the one in PlayEffectAnimationEntity)\nreturn: Same"
+            " as PlayEffectAnimationEntity"
         ),
     )
 
     UpdateStatusIconFlags = Symbol(
         None,
         None,
         None,
@@ -15724,15 +16174,15 @@
         None,
         None,
         (
             "Copies all entries in the floor's monster spawn list that have a sprite"
             " size >= 6 to the specified buffer.\n\nThe parameter in r1 can be used to"
             " specify how many entries are already present in the buffer. Entries added"
             " by this function will be placed after those, and the total returned in r1"
-            " will account for existing entries as well.\n\nr0: (output) Buffer where"
+            " will account for existing entries as well.\n\nr0: [output] Buffer where"
             " the result will be stored\nr1: Current amount of entries in the"
             " buffer\nreturn: New amount of entries in the buffer"
         ),
     )
 
     IsOnMonsterSpawnList = Symbol(
         None,
@@ -16104,14 +16554,26 @@
             " the effect of the Switcher Orb). \n\nThe function checks for the Suction"
             " Cups ability for both the user and the target, and for the Mold Breaker"
             " ability on the user.\n\nr0: pointer to user entity\nr1: pointer to target"
             " entity"
         ),
     )
 
+    SetLeaderActionFields = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the leader's monster::action::action_id to the specified"
+            " value.\n\nAlso sets monster::action::action_use_idx and"
+            " monster::action::field_0xA to 0, as well as monster::action::field_0x10"
+            " and monster::action::field_0x12 to -1.\n\nr0: ID of the action to set"
+        ),
+    )
+
     ClearMonsterActionFields = Symbol(
         None,
         None,
         None,
         (
             "Clears the fields related to AI in the monster's data struct, setting them"
             " all to 0.\nSpecifically, monster::action::action_id,"
@@ -16191,14 +16653,27 @@
         (
             "Sets a monster's action to action::ACTION_REGULAR_ATTACK, with a specified"
             " direction.\n\nr0: Pointer to the monster's action field\nr1: Direction in"
             " which to use the move. Gets stored in monster::action::direction."
         ),
     )
 
+    SetActionUseMovePlayer = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets a monster's action to action::ACTION_USE_MOVE_PLAYER, with a"
+            " specified monster and move index.\n\nr0: Pointer to the monster's action"
+            " field\nr1: Index of the monster that is using the move on the entity"
+            " list. Gets stored in monster::action::action_use_idx.\nr2: Index of the"
+            " move to use (0-3). Gets stored in monster::action::field_0xA."
+        ),
+    )
+
     SetActionUseMoveAi = Symbol(
         None,
         None,
         None,
         (
             "Sets a monster's action to action::ACTION_USE_MOVE_AI, with a specified"
             " direction and move index.\n\nr0: Pointer to the monster's action"
@@ -16345,14 +16820,169 @@
             "If the flag for a trapper trap is set, handles spawning a trap based upon"
             " the\ninformation inside the dungeon struct. Uses the entity for logging a"
             " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
             " true if a trap was spawned succesfully"
         ),
     )
 
+    TryTriggerTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called whenever a monster steps on a trap.\n\nThe function will try to"
+            " trigger it. Nothing will happen if the pokémon has the same team as the"
+            " trap. The attempt to trigger the trap can also fail due to IQ skills, due"
+            " to the trap failing to work (random chance), etc.\n\nr0: Entity who"
+            " stepped on the trap\nr1: Trap position\nr2: ?\nr3: ?"
+        ),
+    )
+
+    ApplyMudTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly lowers attack, special attack, defense, or special defense of the"
+            " defender by 3 stages.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer"
+        ),
+    )
+
+    ApplyStickyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to make something in the bag"
+            " sticky. Otherwise, try to make the item the monster is holding"
+            " sticky.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyGrimyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to turn food items in the"
+            " toolbox into\ngrimy food. Otherwise, try to make the food item the"
+            " monster is holding grimy food.\n\nr0: attacker entity pointer\nr1:"
+            " defender entity pointer"
+        ),
+    )
+
+    ApplyPitfallTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, end the current floor unless it has a"
+            " rescue point.\nOtherwise, make the entity faint and ignore reviver seeds."
+            " If not called by a random\ntrap, break the grate on the pitfall"
+            " trap.\n\nr0: attacker entity pointer\nr1: defender entity pointer\nr2:"
+            " tile pointer\nr3: bool caused by random trap"
+        ),
+    )
+
+    ApplySummonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly spawns 2-4 enemy monsters around the position. The entity is only"
+            " used for\nlogging messages.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyPpZeroTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the PP of one of the defender's moves to 0.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyPokemonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Turns item in the same room as the tile at the position (usually just the"
+            " entities's\nposition) into monsters. If the position is in a hallway,"
+            " convert items in a 3x3 area\ncentered on the position into"
+            " monsters.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTripTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to drop the defender's item and places it on the floor.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyToxicSpikesTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to inflict 10 damage on the defender and then tries to poison"
+            " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyRandomTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Selects a random trap that isn't a wonder tile and isn't a random trap and"
+            " calls\nApplyTrapEffect on all monsters that is different from the trap's"
+            " team.\n\nr0: Triggered trap\nr1: User\nr2: Target, normally same as"
+            " user\nr3: Tile that contains the trap\nstack[0]: position"
+        ),
+    )
+
+    ApplyGrudgeTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Spawns several monsters around the position and gives all monsters on the"
+            " floor the\ngrudge status condition.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Performs the effect of a triggered trap.\n\nThe trap's animation happens"
+            " before this function is called.\n\nr0: Triggered trap\nr1: User\nr2:"
+            " Target, normally same as user\nr3: Tile that contains the trap\nstack[0]:"
+            " position\nstack[1]: trap ID\nstack[2]: bool caused by random"
+            " trap\nreturn: True if the trap should be destroyed after the effect is"
+            " applied"
+        ),
+    )
+
+    RevealTrapsNearby = Symbol(
+        None,
+        None,
+        None,
+        "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16376,28 +17006,63 @@
         None,
         (
             "Returns a pointer to the action data of the current leader (field 0x4A on"
             " its monster struct).\n\nNo params."
         ),
     )
 
+    GetEntityTouchscreenArea = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the area on the touchscreen that contains the sprite of the"
+            " specified entity\n\nr0: Entity pointer\nr1: [output] struct where the"
+            " result should be written"
+        ),
+    )
+
     SetLeaderAction = Symbol(
         None,
         None,
         None,
         (
             "Sets the leader's action field depending on the inputs given by the"
             " player.\n\nThis function also accounts for other special situations that"
             " can force a certain action, such as when the leader is running. The"
             " function also takes care of opening the main menu when X is pressed.\nThe"
             " function generally doesn't return until the player has an action"
             " set.\n\nNo params."
         ),
     )
 
+    ShouldLeaderKeepRunning = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Determines if the leader should keep running. Returns false if the leader"
+            " bumps into something, or if an action that should stop the leader takes"
+            " place.\n\nreturn: True if the leader should keep running, false if it"
+            " should stop."
+        ),
+    )
+
+    CheckLeaderTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the tile the leader just stepped on and performs any required"
+            " actions, such as picking up items, triggering traps, etc.\n\nContains a"
+            " switch that checks the type of the tile the leader just stepped on.\n\nNo"
+            " params."
+        ),
+    )
+
     ChangeLeader = Symbol(
         None,
         None,
         None,
         (
             "Tries to change the current leader to the monster specified by"
             " dungeon::new_leader.\n\nAccounts for situations that can prevent changing"
@@ -16537,14 +17202,25 @@
         (
             "Handles a fainted pokémon (reviving does not count as fainting).\n\nr0:"
             " Fainted entity\nr1: Damage source (move ID or greater than the max move"
             " id for other causes)\nr2: Entity responsible of the fainting"
         ),
     )
 
+    MoveMonsterToPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Moves a monster to the target position. Used both for regular movement and"
+            " special movement (like teleportation).\n\nr0: Entity pointer\nr1: X"
+            " target position\nr2: Y target position\nr3: ?"
+        ),
+    )
+
     UpdateAiTargetPos = Symbol(
         None,
         None,
         None,
         (
             "Given a monster, updates its target_pos field based on its current"
             " position and the direction in which it plans to attack.\n\nr0: Entity"
@@ -16669,14 +17345,24 @@
             "Restores PP for all moves, clears flags move::f_consume_2_pp,"
             " move::flags2_unk5 and move::flags2_unk7, and sets flag"
             " move::f_consume_pp.\nCalled when a monster is revived.\n\nr0: pointer to"
             " entity whose moves will be restored"
         ),
     )
 
+    BoostIQ = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's IQ.\n\nr0: monster entity pointer\nr1: iq"
+            " boost\nr2: bool suppress logs"
+        ),
+    )
+
     ShouldMonsterHeadToStairs = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given monster should try to reach the stairs when controlled"
             " by the AI\n\nr0: Entity pointer\nreturn: True if the monster should try"
@@ -16693,14 +17379,28 @@
             " dungeon::mew_cannot_spawn or the second parameter are true.\n\nCalled"
             " before spawning an enemy, appears to be checking if Mew can spawn on the"
             " current floor.\n\nr0: monster id\nr1: return false if the monster id is"
             " Mew\nreturn: bool"
         ),
     )
 
+    TryEndStatusWithAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if any of the defender's active abilities would end one of their"
+            " current status\nconditions. For example, if the ability Own Tempo will"
+            " stop confusion.\n\nCalled after changing a monster's ability with skill"
+            " swap, role play, or trace to\nremove statuses the monster should no"
+            " longer be affected by.\n\nr0: attacker entity pointer\nr1: defender"
+            " entity pointer"
+        ),
+    )
+
     ExclusiveItemEffectIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is a team member under the effects of a certain"
             " exclusive item effect.\n\nr0: entity pointer\nr1: exclusive item effect"
@@ -16830,14 +17530,27 @@
             "Checks if a monster does not gain experience.\n\nThis basically just"
             " inverts IsSpecialStoryAlly, with the exception of also checking for the"
             " 'Joined At' field being DUNGEON_CLIENT (is this set for mission"
             " clients?).\n\nr0: monster pointer\nreturn: bool"
         ),
     )
 
+    InitOtherMonsterData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes stats, IQ skills and moves for a given monster\n\nMight only"
+            " be used when spawning fixed room monsters.\n\nr0: Entity pointer\nr1:"
+            " Fixed room monster stats index\nr2: Spawn direction? (when calling this"
+            " function while spawning a fixed room monster, this is the parameter value"
+            " associated to the spawn action, after converting it to a direction.)"
+        ),
+    )
+
     SpawnTeam = Symbol(
         None,
         None,
         None,
         "Seems to initialize and spawn the team when entering a dungeon.\n\nr0: ?",
     )
 
@@ -16881,16 +17594,28 @@
     )
 
     InitMonster = Symbol(
         None,
         None,
         None,
         (
-            "Initializes a monster struct.\n\nr0: pointer to monster to initialize\nr1:"
-            " some flag"
+            "Initializes the monster struct within the provided entity struct.\n\nr0:"
+            " ?\nr1: Pointer to the entity whose monster struct should be"
+            " initialized\nr2: pointer to the entity's spawned_monster_data struct\nr3:"
+            " (?) Pointer to something"
+        ),
+    )
+
+    SubInitMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called by InitMonster. Initializes some fields on the monster"
+            " struct.\n\nr0: pointer to monster to initialize\nr1: some flag"
         ),
     )
 
     MarkShopkeeperSpawn = Symbol(
         None,
         None,
         None,
@@ -16995,14 +17720,24 @@
         (
             "Returns the number of attacks that a monster can do in one turn (1 or"
             " 2).\n\nChecks for the abilities Swift Swim, Chlorophyll, Unburden, and"
             " for exclusive items.\n\nr0: pointer to entity\nreturns: int"
         ),
     )
 
+    GetMonsterDisplayNameType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Determines how the name of a monster should be displayed.\n\nr0: Entity"
+            " pointer\nreturn: Display name type"
+        ),
+    )
+
     GetMonsterName = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: buffer\nr1: TargetInfo",
     )
 
@@ -17153,14 +17888,39 @@
         None,
         (
             "Checks if a monster has the sleep, nightmare, or napping status.\n\nr0:"
             " entity pointer\nreturn: bool"
         ),
     )
 
+    CanMonsterMoveInDirection = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the given monster can move in the specified direction\n\nReturns"
+            " false if any monster is standing on the target tile\n\nr0: Monster entity"
+            " pointer\nr1: Direction to check\nreturn: bool"
+        ),
+    )
+
+    GetFinalMobilityType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the mobility type of a monster, after accounting for things that"
+            " could affect it (like items or IQ skills)\n\nIf the specified direction"
+            " is DIR_NONE, direction checks are skipped. If it's not,"
+            " MOBILITY_INTANGIBLE is only returned if the direction is not"
+            " diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility type\nr2:"
+            " Direction of mobility\nreturn: Final mobility type"
+        ),
+    )
+
     IsMonsterCornered = Symbol(
         None,
         None,
         None,
         (
             "True if the given monster is cornered (it can't move in any"
             " direction)\n\nr0: Entity pointer\nreturn: True if the monster can't move"
@@ -17188,15 +17948,15 @@
         None,
         None,
         (
             "Checks whether an AI-controlled monster can move in the specified"
             " direction.\nAccounts for walls, other monsters on the target position and"
             " IQ skills that might prevent a monster from moving into a specific"
             " location, such as House Avoider, Trap Avoider or Lava Evader.\n\nr0:"
-            " Entity pointer\nr1: Direction\nr2: (output) True if movement was not"
+            " Entity pointer\nr1: Direction\nr2: [output] True if movement was not"
             " possible because there was another monster on the target tile, false"
             " otherwise.\nreturn: True if the monster can move in the specified"
             " direction, false otherwise."
         ),
     )
 
     ShouldMonsterRunAway = Symbol(
@@ -17216,14 +17976,47 @@
         (
             "Calls ShouldMonsterRunAway and returns its result. It also calls another"
             " function if the result was true.\n\nr0: Entity pointer\nr1: ?\nreturn:"
             " Result of the call to ShouldMonsterRunAway"
         ),
     )
 
+    SafeguardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Safeguard.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: flag to log a message\nreturn:"
+            " bool"
+        ),
+    )
+
+    LeafGuardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is protected by the ability Leaf Guard.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer\nr2: flag to log a"
+            " message\nreturn: bool"
+        ),
+    )
+
+    IsProtectedFromStatDrops = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting their stats dropped"
+            " by the user.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     NoGastroAcidStatus = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster does not have the Gastro Acid status.\n\nr0: entity"
             " pointer\nreturn: bool"
@@ -17384,14 +18177,25 @@
             "Updates monster::state_flags and monster::prev_state_flags with new"
             " values.\n\nr0: monster pointer\nr1: bitmask for bits to update\nr2:"
             " whether to set the bits indicated by the mask to 1 or 0\nreturn: whether"
             " or not any of the masked bits changed from the previous state"
         ),
     )
 
+    IsProtectedFromNegativeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting a negative status"
+            " condition.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     AddExpSpecial = Symbol(
         None,
         None,
         None,
         (
             "Adds to a monster's experience points, subject to experience boosting"
             " effects.\n\nThis function appears to be called only under special"
@@ -17405,17 +18209,31 @@
     )
 
     EnemyEvolution = Symbol(
         None,
         None,
         None,
         (
-            "Checks if the specified enemy should evolve because it just defeated an"
-            " ally, and if so, attempts to evolve it.\n\nr0: Pointer to the enemy to"
-            " check"
+            "Checks if any enemies on the floor should evolve and attempts to evolve"
+            " it. The\nentity pointer passed seems to get replaced by a generic"
+            " placeholder entity if the\nentity pointer passed is invalid.\n\nr0:"
+            " entity pointer"
+        ),
+    )
+
+    LevelUpItemEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to level up the the target. Calls LevelUp with a few extra checks"
+            " and messages\nfor using as an item. Used for the Joy Seed and Golden"
+            " Seed.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: number"
+            " of levels\nr3: bool message flag?\nstack[0]: bool show level up dialog"
+            " (for example 'Hey, I leveled up!' with a portrait)?"
         ),
     )
 
     TryDecreaseLevel = Symbol(
         None,
         None,
         None,
@@ -17427,27 +18245,31 @@
     )
 
     LevelUp = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: user entity"
-            " pointer\nr1: target entity pointer\nr2: message flag?\nr3: ?\nreturn:"
-            " success flag?"
+            "Attempts to level up the the target. Fails if the target's level can't be"
+            " raised. The show show level up dialog bool does nothing for monsters not"
+            " on the team.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " bool message flag?\nr3: bool show level up dialog (for example 'Hey, I"
+            " leveled up!' with a portrait)?\nreturn: success flag"
         ),
     )
 
     EvolveMonster = Symbol(
         None,
         None,
         None,
         (
-            "Makes the specified monster evolve into the specified species.\n\nr0:"
-            " Pointer to the entity to evolve\nr1: ?\nr2: Species to evolve into"
+            "Makes the specified monster evolve into the specified species. Has a"
+            " special case when\na monster evolves into Ninjask and tries to spawn a"
+            " Shedinja as well.\n\nr0: user entity pointer?\nr1: target pointer to the"
+            " entity to evolve\nr2: Species to evolve into"
         ),
     )
 
     GetSleepAnimationId = Symbol(
         None,
         None,
         None,
@@ -17469,14 +18291,58 @@
             " example, this delayed display system is used to display multiple monsters"
             " moving at once even though they take turns sequentially.\n\nr0: Pointer"
             " to an entity. Can be null.\nreturns: Seems to be true if there were any"
             " pending actions to display."
         ),
     )
 
+    CheckNonLeaderTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Similar to CheckLeaderTile, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: Entity pointer"
+        ),
+    )
+
+    EndNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Cures the target's negative status conditions. The game rarely (if not"
+            " never) calls\nthis function with the bool to remove the wrapping status"
+            " false.\n\nr0: pointer to user\nr1: pointer to target\nr2: bool play"
+            " animation\nr3: bool log failure message\nstack[0]: bool remove wrapping"
+            " status\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    EndNegativeStatusConditionWrapper = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EndNegativeStatusCondition with remove wrapping status false.\n\nr0:"
+            " pointer to user\nr1: pointer to target\nr2: bool play animation\nr3: bool"
+            " log failure message\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    TransferNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Transfers all negative status conditions the user has and gives then to"
+            " the target.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     EndSleepClassStatus = Symbol(
         None,
         None,
         None,
         (
             "Cures the target's sleep, sleepless, nightmare, yawn or napping status due"
             " to the action of the user, and prints the event to the log.\n\nr0:"
@@ -17582,14 +18448,25 @@
         (
             "Removes the target's magnet rise status due to the action of the user, and"
             " prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
             " target"
         ),
     )
 
+    TransferNegativeBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to transfer the the negative blinker class status conditions from"
+            " the user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer\nreturn: Whether or not the status could be transferred"
+        ),
+    )
+
     TryTriggerMonsterHouse = Symbol(
         None,
         None,
         None,
         (
             "Triggers a Monster House for an entity, if the right conditions are"
             " met.\n\nConditions: entity is valid and on the team, the tile is a"
@@ -18017,14 +18894,26 @@
         (
             "Inflicts the Sleep status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
             " number of turns\nr3: flag to log a message on failure"
         ),
     )
 
+    IsProtectedFromSleepClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is immune to sleep class status conditions.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nr2: ignore safeguard\nr3:"
+            " ignore other protections (exclusive items + leaf guard)\nstack[0]: flag"
+            " to log a message on failure\nreturn: bool"
+        ),
+    )
+
     TryInflictNightmareStatus = Symbol(
         None,
         None,
         None,
         (
             "Inflicts the Nightmare status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
@@ -18527,91 +19416,638 @@
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
             " to log a message on failure\nr3: flag to only perform the check for"
             " inflicting without actually inflicting\nreturn: Whether or not the status"
             " could be inflicted"
         ),
     )
 
-    TryInflictDestinyBond = Symbol(
+    TryInflictDestinyBondStatus = Symbol(
         None,
         None,
         None,
         (
             "Inflicts the Destiny Bond status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
-    TryInvisify = Symbol(
+    TryInflictSureShotStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Sure Shot status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWhifferStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Whiffer status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSetDamageStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Set Damage status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictFocusEnergyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Focus Energy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictDecoyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Decoy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictCurseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Curse status condition on a target monster if possible and if"
+            " the user is\na ghost type. Otherwise, just boost the user's defense and"
+            " attack then lower the user's\nspeed.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
+    TryInflictSnatchStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Snatch status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictTauntStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Taunt status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictStockpileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Stockpile condition on a target monster if possible. Won't"
+            " boost the level\nof stockpiling above 3.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nreturn: Whether or not the status could be"
+            " inflicted or boosted"
+        ),
+    )
+
+    TryInflictInvisibleStatus = Symbol(
         None,
         None,
         None,
         (
             "Attempts to turn the target invisible.\n\nThe user pointer is only used"
             " when calling LogMessage functions.\n\nr0: user entity pointer\nr1: target"
             " entity pointer"
         ),
     )
 
+    TryInflictPerishSongStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Perish Song status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEncoreStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Encore status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryDecreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the belly size of the target. Only when max belly shrink"
+            " is 0, the\ncurrent belly is reduced by belly to lose. If both are"
+            " non-zero, only the max belly\nshrink is applied.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: belly to lose\nr3: max belly"
+            " shrink"
+        ),
+    )
+
+    TryIncreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restore belly and possibly boost max belly of the target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " belly to restore\nr3: max belly boost (if belly is full)\nstack[0]: flag"
+            " to log a message"
+        ),
+    )
+
+    TryInflictMuzzledStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Muzzled status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
     TryTransform = Symbol(
         None,
         None,
         None,
         (
             "Attempts to transform the target into the species of a random monster"
             " contained in the list returned by MonsterSpawnListPartialCopy.\n\nThe"
             " user pointer is only used when calling LogMessage functions.\n\nr0: user"
             " entity pointer\nr1: target entity pointer"
         ),
     )
 
+    TryInflictMobileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mobile status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictExposedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Exposed status condition on a target monster if possible."
+            " Only applies to\nGhost types and monsters with raised evasion. If the"
+            " animation effect ID is 0,\ndefaults to animation ID 0xE (this fallback"
+            " animation likely can't be seen in normal\nplay).\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: animation effect ID\nr3: flag to"
+            " only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryActivateIdentifyCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the flag for the identify orb which causes monsters holding items to"
+            " be shown with\na blue exclamation mark status icon.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictBlinkerStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Blinker status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting\nr3:"
+            " flag to log a message on failure\nreturn: Whether or not the status could"
+            " be inflicted"
+        ),
+    )
+
     IsBlinded = Symbol(
         None,
         None,
         None,
         (
             "Returns true if the monster has the blinded status (see"
             " statuses::blinded), or if it is not the leader and is holding Y-Ray"
             " Specs.\n\nr0: pointer to entity\nr1: flag for whether to check for the"
             " held item\nreturn: bool"
         ),
     )
 
+    TryInflictCrossEyedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Cross-Eyed status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEyedropStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Eyedrop status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSlipStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Slip status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nreturn: Whether or not"
+            " the status could be inflicted"
+        ),
+    )
+
+    TryInflictDropeyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Dropeye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
     RestoreMovePP = Symbol(
         None,
         None,
         None,
         (
             "Restores the PP of all the target's moves by the specified amount.\n\nr0:"
             " user entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3:"
             " flag to suppress message logging"
         ),
     )
 
-    SetReflectDamageCountdownTo4 = Symbol(
+    ApplyProteinEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: attack boost"
+        ),
+    )
+
+    ApplyCalciumEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's special attack stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special attack boost"
+        ),
+    )
+
+    ApplyIronEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's defense stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: defense boost"
+        ),
+    )
+
+    ApplyZincEffect = Symbol(
         None,
         None,
         None,
         (
-            "Sets the monster's reflect damage countdown to a global value"
+            "Tries to boost the target's special defense stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special defense boost"
+        ),
+    )
+
+    TryInflictLongTossStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Long Toss status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictPierceStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Pierce status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictGastroAcidStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Gastro Acid status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    SetAquaRingHealingCountdownTo4 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the countdown for Aqua Ring healing countdown to a global value"
             " (0x4).\n\nr0: pointer to entity"
         ),
     )
 
+    ApplyAquaRingHealing = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the passive healing gained from the Aqua Ring status.\n\nr0:"
+            " pointer to entity"
+        ),
+    )
+
+    TryInflictAquaRingStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Aqua Ring status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLuckyChantStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Lucky Chant status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictHealBlockStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Heal Block status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    MonsterHasEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the monster has the Embargo status condition.\n\nr0:"
+            " pointer to entity\nreturn: bool"
+        ),
+    )
+
+    LogItemBlockedByEmbargo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Logs the error message when the usage of an item is blocked by"
+            " Embargo.\n\nr0: pointer to entity"
+        ),
+    )
+
+    TryInflictEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Embargo status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictMiracleEyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Miracle Eye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting"
+        ),
+    )
+
+    TryInflictMagnetRiseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magnet Rise status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     HasConditionalGroundImmunity = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    TryInflictSafeguardStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Safeguard status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMistStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mist status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWishStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Wish status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMagicCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magic Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLightScreenStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Light Screen status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictReflectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Reflect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Protect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictEndureStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Endure status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorMoveStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Move status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictConversion2Status = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Conversion2 status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictVitalThrowStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Vital Throw status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryResetStatChanges = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reset the stat changes of the defender.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr3: bool to force animation"
+        ),
+    )
+
     MirrorMoveIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
             " the effects is a status, 2 if it comes from an exclusive item, 0"
@@ -18769,21 +20205,101 @@
         (
             "Seems to apply an item's effect via a giant switch statement?\n\nr3:"
             " attacker pointer\nstack[0]: defender pointer\nstack[1]: thrown item"
             " pointer\nothers: ?"
         ),
     )
 
-    ViolentSeedBoost = Symbol(
+    ApplyCheriBerryEffect = Symbol(
         None,
         None,
         None,
         (
-            "Applies the Violent Seed boost to an entity.\n\nr0: attacker pointer\nr1:"
-            " defender pointer"
+            "Tries to heal the paralysis status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyPechaBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the poisoned and badly poisoned status condition. Prints a"
+            " message on\nfailure.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyRawstBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the burn status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyHungerSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Empties the targets belly to cause Hungry Pal status in non-leader"
+            " monsters and\nFamished in the leader monster.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyVileSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Reduces the targets defense and special defense stages to the lowest"
+            " level.\n\nr0: attacker pointer\nr1: defender pointer"
+        ),
+    )
+
+    ApplyViolentSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the target's offensive stats stages to the max.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGinsengEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the power of the move at the top of the target's Move List. Appears"
+            " to have a\nleftover check to boost the power of a move by 3 instead of 1"
+            " that always fails because\nthe chance is 0.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyBlastSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If thrown, unfreeze and deal fixed damage to the defender. If not thrown,"
+            " try to find \na monster in front of the attacker. If a monster is found"
+            " unfreeze and dedal fixed \ndamage to the defender. Appears to have a"
+            " leftover check for if the current fixed room is a boss fight and loads a"
+            " different pointer for the damage when used in a boss room.\nHowever, this"
+            " isn't noticeable because both the normal and boss damage is the"
+            " same.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: bool"
+            " thrown"
         ),
     )
 
     ApplyGummiBoostsDungeonMode = Symbol(
         None,
         None,
         None,
@@ -18825,14 +20341,68 @@
         None,
         (
             "If the target monster is a Linoone, restores all the PP of all the"
             " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
+    ApplyDoughSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a team member, set dough_seed_extra_poke_flag to"
+            " true to \nmake extra poke spawn on the next floor. Otherwise, do"
+            " nothing.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyViaSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to randomly teleport the target with a message for eating the"
+            " seed.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGravelyrockEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restores 10 hunger to the target and will raise the target's IQ if they"
+            " are a bonsly\nor sudowoodo.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyGonePebbleEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Causes a few visual effects, temporarily changes the dungeon music to the"
+            " Goodnight\ntrack, and gives the target the enduring status.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGracideaEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target is Shaymin, attempt to change the target's form to Shaymin"
+            " Sky Forme. Otherwise, do nothing.\n\nr0: user entity pointer\nr1: target"
+            " entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -18906,15 +20476,29 @@
         None,
         None,
         None,
         (
             "Creates an explosion if possible.\n\nThe target monster is considered the"
             " source of the explosion.\n\nr0: user entity pointer\nr1: target entity"
             " pointer\nr2: coordinates where the explosion should take place"
-            " (unverified)\nr3: ?\nstack[0]: ?\nstack[1]: damage source (normally"
+            " (center)\nr3: explosion radius (only works correctly with 1 and"
+            " 2)\nstack[0]: damage type\nstack[1]: damage source"
+        ),
+    )
+
+    TryAftermathExplosion = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Creates the explosion for the ability aftermath if possible.\n\nThe target"
+            " monster is considered the source of the explosion.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: coordinates where the explosion"
+            " should take place (center)\nr3: explosion radius (only works correctly"
+            " with 1 and 2)\nstack[0]: damage type\nstack[1]: damage source (normally"
             " DAMAGE_SOURCE_EXPLOSION)"
         ),
     )
 
     TryWarp = Symbol(
         None,
         None,
@@ -19382,14 +20966,57 @@
     GetStairsRoom = Symbol(
         None,
         None,
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    UpdateTrapsVisibility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Exact purpose unknown. Gets called whenever a trap tile is shown or"
+            " hidden.\n\nNo params."
+        ),
+    )
+
+    DrawTileGrid = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Draws a grid on the nearby walkable tiles. Triggered by pressing Y.\n\nr0:"
+            " Coordinates of the entity around which the grid will be drawn\nr1: ?\nr2:"
+            " ?\nr3: ?"
+        ),
+    )
+
+    HideTileGrid = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Hides the grid on the nearby walkable tiles. Triggered by releasing"
+            " Y.\n\nNo params."
+        ),
+    )
+
+    DiscoverMinimap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Discovers the tiles around the specified position on the minimap.\n\nThe"
+            " discovery radius depends on the visibility range of the floor. If"
+            " display_data::blinded is true, the function returns early without doing"
+            " anything.\n\nr0: Position around which the map should be discovered"
+        ),
+    )
+
     IsWaterTileset = Symbol(
         None,
         None,
         None,
         (
             "Returns flag tileset_property::is_water_tileset for the current"
             " tileset\n\nreturn: True if the current tileset is a water tileset"
@@ -19455,14 +21082,34 @@
         (
             "Sets the boost_kecleon_shop_spawn_chance field on the dungeon struct"
             " depending on if a team member has the exclusive item effect for more"
             " kecleon shops.\n\nNo params."
         ),
     )
 
+    SetDoughSeedFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the dough_seed_extra_money_flag field on the dungeon struct to the"
+            " given value.\n\nr0: bool to set the flag to"
+        ),
+    )
+
+    TrySpawnDoughSeedPoke = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the dough_seed_extra_money_flag field on the dungeon struct and"
+            " tries to spawn\nextra poke if it is set.\n\nNo params."
+        ),
+    )
+
     IsSecretBazaar = Symbol(
         None,
         None,
         None,
         "Checks if the current floor is the Secret Bazaar.\n\nreturn: bool",
     )
 
@@ -19513,28 +21160,62 @@
         None,
         (
             "Checks if the current floor is a secret bazaar or a secret"
             " room.\n\nreturn: bool"
         ),
     )
 
+    HiddenStairsPresent = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the hidden stairs are present on this floor.\n\nThe function"
+            " checks that dungeon_generation_info::hidden_stairs_pos isn't (-1,"
+            " -1)\n\nreturn: True if the hidden stairs are present on this floor, false"
+            " otherwise."
+        ),
+    )
+
+    HiddenStairsTrigger = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called whenever the leader steps on the hidden stairs.\n\nIf the stairs"
+            " hadn't been revealed yet, plays the corresponding animation.\n\nr0: True"
+            " to display a message if the stairs are revealed, false to omit it."
+        ),
+    )
+
     GetDungeonGenInfoUnk0C = Symbol(
         None, None, None, "return: dungeon_generation_info::field_0xc"
     )
 
     GetMinimapData = Symbol(
         None,
         None,
         None,
         (
             "Returns a pointer to the minimap_display_data struct in the dungeon"
             " struct.\n\nreturn: minimap_display_data*"
         ),
     )
 
+    DrawMinimapTile = Symbol(
+        None,
+        None,
+        None,
+        "Draws a single tile on the minimap.\n\nr0: X position\nr1: Y position",
+    )
+
+    UpdateMinimap = Symbol(
+        None, None, None, "Graphically updates the minimap\n\nNo params."
+    )
+
     SetMinimapDataE447 = Symbol(
         None,
         None,
         None,
         (
             "Sets minimap_display_data::field_0xE447 to the specified value\n\nr0:"
             " Value to set the field to"
@@ -19558,14 +21239,35 @@
         None,
         (
             "Sets minimap_display_data::field_0xE448 to the specified value\n\nr0:"
             " Value to set the field to"
         ),
     )
 
+    InitWeirdMinimapMatrix = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the matrix at minimap_display_data+0xE000. Seems to overflow"
+            " said matrix when doing so.\n\nNo params."
+        ),
+    )
+
+    InitMinimapDisplayTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to initialize an instance of struct minimap_display_tile\n\nr0:"
+            " Pointer to struct to init\nr1: Seems to be a pointer to the file that"
+            " stores minimap icons or something like that"
+        ),
+    )
+
     LoadFixedRoomDataVeneer = Symbol(
         None,
         None,
         None,
         (
             "Likely a linker-generated veneer for LoadFixedRoomData.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nNo"
@@ -20257,14 +21959,24 @@
             " reached by the traversal algorithm, then the stairs must not be reachable"
             " from that tile.\n\nr0: x coordinate of the stairs\nr1: y coordinate of"
             " the stairs\nr2: flag to always return true, but set a special bit on all"
             " walkable tiles that aren't reachable from the stairs\nreturn: bool"
         ),
     )
 
+    GetNextFixedRoomAction = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the next action that needs to be performed when spawning a fixed"
+            " room tile.\n\nreturn: Next action ID"
+        ),
+    )
+
     ConvertWallsToChasms = Symbol(
         None, None, None, "Converts all wall tiles to chasms.\n\nNo params."
     )
 
     ResetInnerBoundaryTileRows = Symbol(
         None,
         None,
@@ -20315,25 +22027,75 @@
             " HIDDEN_STAIRS_RANDOM_SECRET_BAZAAR_OR_SECRET_ROOM and the"
             " floor_properties::hidden_stairs_spawn_chance) into a concrete hidden"
             " stairs type.\n\nr0: dungeon generation info pointer\nr1: floor properties"
             " pointer\nreturn: enum hidden_stairs_type"
         ),
     )
 
+    GetFinalKecleonShopSpawnChance = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the kecleon shop spawn chance for the floor.\n\nWhen"
+            " dungeon::boost_kecleon_shop_spawn_chance is false, returns the same value"
+            " as the input. When it's true, returns the input (chance * 1.2).\n\nr0:"
+            " base kecleon shop spawn chance,"
+            " floor_properties::kecleon_shop_spawn_chance\nreturn: int"
+        ),
+    )
+
     ResetHiddenStairsSpawn = Symbol(
         None,
         None,
         None,
         (
             "Resets hidden stairs spawn information for the floor. This includes the"
             " position on the floor generation status as well as the flag indicating"
             " whether the spawn was blocked.\n\nNo params."
         ),
     )
 
+    PlaceFixedRoomTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to spawn a single tile when generating a fixed room. The tile might"
+            " contain an item or a monster.\n\nr0: Pointer to the tile to spawn\nr1:"
+            " Fixed room action to perform. Controls what exactly will be spawned. The"
+            " action is actually 12 bits long, the highest 4 bits are used as a"
+            " parameter that represents a direction (for example, when spawning a"
+            " monster).\nr2: Tile X position\nr3: Tile Y position"
+        ),
+    )
+
+    FixedRoomActionParamToDirection = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Converts the parameter stored in a fixed room action value to a direction"
+            " ID.\n\nThe conversion is performed by subtracting 1 to the value. If the"
+            " parameter had a value of 0, DIR_NONE is returned.\n\nr0: Parameter"
+            " value\nreturn: Direction"
+        ),
+    )
+
+    ApplyKeyEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to open a locked door in front of the target if a locked door has"
+            " not already\nbeen open on the floor.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
     LoadFixedRoomData = Symbol(
         None,
         None,
         None,
         (
             "Loads fixed room data from BALANCE/fixed.bin into the buffer pointed to by"
             " FIXED_ROOM_DATA_PTR.\n\nNo params."
@@ -21107,15 +22869,27 @@
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
             " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
-    OpenMenu = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
+    OpenMenu = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Opens a menu. The menu to open depends on the specified parameter.\n\nIt"
+            " looks like the function takes a parameter in r0, but doesn't use it. r1"
+            " doesn't even get set when this function is called.\n\nr0: (?) Unused by"
+            " the function. Seems to be 1 byte long.\nr1: (?) Unused by the function."
+            " Seems to be 1 byte long.\nr2: True to open the bag menu, false to open"
+            " the main dungeon menu"
+        ),
+    )
 
     OthersMenuLoop = Symbol(
         None,
         None,
         None,
         (
             "Called on each frame while the in-dungeon 'others' menu is open.\n\nIt"
@@ -21290,27 +23064,27 @@
         None,
         (
             "The move target and range code for special healing moves that target just"
             " the user (0x273).\n\ntype: struct move_target_and_range (+ padding)"
         ),
     )
 
-    PLAIN_SEED_VALUE = Symbol(
-        None, None, None, "Some value related to the Plain Seed (0xBE9)."
+    PLAIN_SEED_STRING_ID = Symbol(
+        None, None, None, "The string ID for eating a Plain Seed (0xBE9)."
     )
 
     MAX_ELIXIR_PP_RESTORATION = Symbol(
         None,
         None,
         None,
         "The amount of PP restored per move by ingesting a Max Elixir (0x3E7).",
     )
 
-    SLIP_SEED_VALUE = Symbol(
-        None, None, None, "Some value related to the Slip Seed (0xC75)."
+    SLIP_SEED_FAIL_STRING_ID = Symbol(
+        None, None, None, "The string ID for when eating the Slip Seed fails (0xC75)."
     )
 
     ROCK_WRECKER_MOVE_ID = Symbol(
         None, None, None, "The move ID for Rock Wrecker (453)."
     )
 
     CASTFORM_NORMAL_FORM_MALE_ID = Symbol(
@@ -22055,15 +23829,28 @@
     loadaddress = None
     length = None
     functions = JpItcmOverlay3Functions
     data = JpItcmOverlay3Data
 
 
 class JpItcmOverlay30Functions:
-    pass
+    WriteQuicksaveData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Function responsible for writing dungeon data when quicksaving.\n\nAmong"
+            " other things, it contains a loop that goes through all the monsters in"
+            " the current dungeon, copying their data to the buffer. The data is not"
+            " copied as-is though, the game uses a reduced version of the monster"
+            " struct containing only the minimum required data to resume the game"
+            " later.\n\nr0: Pointer to buffer where data should be written\nr1: Buffer"
+            " size. Seems to be 0x5800 (22 KB) when the function is called."
+        ),
+    )
 
 
 class JpItcmOverlay30Data:
     OVERLAY30_JP_STRING_1 = Symbol(None, None, None, "みさき様")
 
     OVERLAY30_JP_STRING_2 = Symbol(None, None, None, "やよい様")
```

## pmdsky_debug_py/na.py

```diff
@@ -1033,17 +1033,17 @@
 
     LoadFileInPackWithPackId = Symbol(
         [0xC35C],
         [0x200C35C],
         None,
         (
             "Call LoadFileInPack after looking up the global Pack archive by its"
-            " identifier\n\nr0: pack file identifier\nr1: [output] target buffer\nr2:"
-            " file index\nreturn: number of read bytes (identical to the length of the"
-            " pack from the Table of Content)"
+            " identifier\n\nr0: pack file identifier\nr1: file index\nr2: [output]"
+            " target buffer\nreturn: number of read bytes (identical to the length of"
+            " the pack from the Table of Content)"
         ),
     )
 
     AllocAndLoadFileInPack = Symbol(
         [0xC388],
         [0x200C388],
         None,
@@ -1084,14 +1084,27 @@
             "Load the indexed file from the Pack archive, itself loaded from the"
             " ROM.\n\nr0: pack file struct\nr1: [output] target buffer\nr2: file"
             " index\nreturn: number of read bytes (identical to the length of the pack"
             " from the Table of Content)"
         ),
     )
 
+    GetDungeonResultMsg = Symbol(
+        [0xC4FC],
+        [0x200C4FC],
+        None,
+        (
+            "Gets the message that is shown on the dungeon results ('The Last Outing')"
+            " screen, right after the leader's name.\n\nr0: Damage source value to use"
+            " when displaying the cause of fainting or the result of the"
+            " expedition\nr1: [output] Buffer where the resulting message will be"
+            " stored\nr2: Buffer size\nr3: (?) Seems to point to a buffer"
+        ),
+    )
+
     GetDamageSource = Symbol(
         [0xCA54],
         [0x200CA54],
         None,
         (
             "Gets the damage source for a given move-item combination.\n\nIf there's no"
             " item, the source is the move ID. If the item is an orb, return"
@@ -1169,14 +1182,26 @@
         None,
         (
             "Checks if an item is one of the aura bows received at the start of the"
             " game.\n\nr0: item ID\nreturn: bool"
         ),
     )
 
+    IsTreasureBox = Symbol(
+        [0xCC84],
+        [0x200CC84],
+        None,
+        (
+            "Checks if the given item ID is a treasure box\n\nIn particular, it checks"
+            " if the category of the item is CATEGORY_TREASURE_BOXES_1,"
+            " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
+            " ID\nreturn: True if the item is a treasure box, false otherwise"
+        ),
+    )
+
     InitItem = Symbol(
         [0xCE9C],
         [0x200CE9C],
         None,
         (
             "Initialize an item struct with the given information.\n\nThis will resolve"
             " the quantity based on the item type. For Poké, the quantity code will"
@@ -1496,22 +1521,21 @@
     GetItemMoveId = Symbol(
         [0xEA80],
         [0x200EA80],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: move ID",
     )
 
-    TestItemFlag0xE = Symbol(
+    TestItemAiFlag = Symbol(
         [0xEAA0],
         [0x200EAA0],
         None,
         (
-            "Tests bit 7 if r1 is 0, bit 6 if r1 is 1, bit 5 otherwise\n\nNote:"
-            " unverified, ported from Irdkwia's notes\n\nr0: item ID\nr1:"
-            " bit_id\nreturn: bool"
+            "Used to check the AI flags for an item. Tests bit 7 if r1 is 0, bit 6 if"
+            " r1 is 1, bit\n5 otherwise.\n\nr0: item ID\nr1: bit_id\nreturn: bool"
         ),
     )
 
     IsItemInTimeDarkness = Symbol(
         [0xEB30],
         [0x200EB30],
         None,
@@ -1549,14 +1573,25 @@
         None,
         (
             "Sets the amount of money the player is carrying, clamping the value to the"
             " range [0, MAX_MONEY_CARRIED].\n\nr0: new value"
         ),
     )
 
+    AddMoneyCarried = Symbol(
+        [0xED58],
+        [0x200ED58],
+        None,
+        (
+            "Adds the amount of money to the player's current amount of money. Just"
+            " calls\nSetMoneyCarried with the current money + money gained.\n\nr0:"
+            " money gained (can be negative)"
+        ),
+    )
+
     GetCurrentBagCapacity = Symbol(
         [0xED84],
         [0x200ED84],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: bag capacity",
     )
 
@@ -1577,15 +1612,18 @@
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: # items",
     )
 
     CountNbItemsOfTypeInBag = Symbol(
         [0xEE4C],
         [0x200EE4C],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: count",
+        (
+            "Returns the number of items of the given kind in the bag\n\nr0: item"
+            " ID\nreturn: count"
+        ),
     )
 
     CountItemTypeInBag = Symbol(
         [0xEE88],
         [0x200EE88],
         None,
         (
@@ -1806,14 +1844,24 @@
     ScriptSpecialProcess0x39 = Symbol(
         [0xFD54],
         [0x200FD54],
         None,
         "Implements SPECIAL_PROC_0x39 (see ScriptSpecialProcessCall).\n\nreturn: bool",
     )
 
+    CountNbItemsOfTypeInStorage = Symbol(
+        [0xFEA8],
+        [0x200FEA8],
+        None,
+        (
+            "Returns the number of items of the given kind in the storage\n\nr0: item"
+            " ID\nreturn: count"
+        ),
+    )
+
     CountItemTypeInStorage = Symbol(
         [0xFEE4],
         [0x200FEE4],
         None,
         (
             "Implements SPECIAL_PROC_COUNT_ITEM_TYPE_IN_STORAGE (see"
             " ScriptSpecialProcessCall).\n\nr0: pointer to an owned_item\nreturn:"
@@ -2675,38 +2723,62 @@
     )
 
     DeleteWanTableEntry = Symbol(
         [0x1D1DC],
         [0x201D1DC],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
+            "Always delete an entry if the file is allocated externally"
+            " (file_externally_allocated is set), otherwise, decrease the reference"
+            " counter. If it reach 0, delete the sprite.\n\nr0: wan_table_ptr\nr1:"
             " wan_id"
         ),
     )
 
+    AllocateWanTableEntry = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return the identifier to a free wan table entry (-1 if none are"
+            " avalaible). The entry is zeroed.\n\nr0: wan_table_ptr\nreturn: the entry"
+            " id in wan_table"
+        ),
+    )
+
     FindWanTableEntry = Symbol(
         [0x1D2D4],
         [0x201D2D4],
         None,
         (
-            "Appears to search in the given table (in practice always seems to be"
+            "Search in the given table (in practice always seems to be"
             " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
             " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
             " if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         [0x1D334],
         [0x201D334],
         None,
         (
-            "wan_id = -1 if it is not loaded\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: wan_table_ptr\nr1: bin_file_id\nr2: file_id\nreturn: wan_id"
+            "Look up a sprite with the provided pack_id and file_index in the wan"
+            " table.\n\nr0: wan_table_ptr\nr1: pack_id\nr2: file_index\nreturn: sprite"
+            " id in the wan table, -1 if not found"
+        ),
+    )
+
+    InitWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the input WAN table with 0x60 free entries (it needs a length"
+            " of 0x1510 bytes)\n\nr0: wan_table_ptr"
         ),
     )
 
     LoadWanTableEntry = Symbol(
         [0x1D3DC],
         [0x201D3DC],
         None,
@@ -2714,14 +2786,40 @@
             "Appears to load data from the given file (in practice always seems to be"
             " animation data), using previously loaded data in the given table (see"
             " FindWanTableEntry) if possible.\n\nr0: table pointer\nr1: file name\nr2:"
             " flags\nreturn: table index of the loaded data"
         ),
     )
 
+    LoadWanTableEntryFromPack = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3: allocation"
+            " flags\nstack[0]: compressed\nreturn: the entry id in wan_table"
+        ),
+    )
+
+    LoadWanTableEntryFromPackUseProvidedMemory = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite into the"
+            " provided memory area. Mark the sprite as externally allocated.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3:"
+            " sprite_storage_ptr\nstack[0]: compressed\nreturn: the entry id in"
+            " wan_table"
+        ),
+    )
+
     ReplaceWanFromBinFile = Symbol(
         [0x1D684],
         [0x201D684],
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
             " wan_id\nr2: bin_file_id\nr3: file_id\nstack[0]: compressed"
@@ -2980,14 +3078,30 @@
         [0x24360], [0x2024360], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetStringPower = Symbol(
         [0x24428], [0x2024428], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    GetDungeonResultString = Symbol(
+        [0x24FD8],
+        [0x2024FD8],
+        None,
+        (
+            "Returns a string containing some information to be used when displaying"
+            " the dungeon results screen.\n\nThe exact string returned depends on the"
+            " value of r0:\n0: Name of the move that fainted the leader. Empty string"
+            " if the leader didn't faint.\n1-3: Seems to always result in an empty"
+            " string.\n4: Name of the pokémon that fainted the leader, or name of the"
+            " leader if the leader didn't faint.\n5: Name of the fainted leader. Empty"
+            " string if the leader didn't faint.\n\nr0: String to return\nreturn:"
+            " Pointer to resulting string"
+        ),
+    )
+
     SetQuestionMarks = Symbol(
         [0x250E4],
         [0x20250E4],
         None,
         (
             "Fills the buffer with the string '???'\n\nNote: unverified, ported from"
             " Irdkwia's notes\n\nr0: buffer"
@@ -3313,15 +3427,15 @@
 
     IsMenuOptionActive = Symbol(
         [0x32474],
         [0x2032474],
         None,
         (
             "Called whenever a menu option is selected. Returns whether the option is"
-            " active or not.\n\nr0: ?\nReturn: True if the menu option is enabled,"
+            " active or not.\n\nr0: ?\nreturn: True if the menu option is enabled,"
             " false otherwise."
         ),
     )
 
     ShowKeyboard = Symbol(
         [0x367F0],
         [0x20367F0],
@@ -3705,14 +3819,24 @@
         None,
         (
             "Gets the special episode type from the SPECIAL_EPISODE_TYPE script"
             " variable.\n\nreturn: special episode type"
         ),
     )
 
+    GetExecuteSpecialEpisodeType = Symbol(
+        [0x4C938],
+        [0x204C938],
+        None,
+        (
+            "Gets the special episode type from the EXECUTE_SPECIAL_EPISODE_TYPE script"
+            " variable.\n\nreturn: special episode type"
+        ),
+    )
+
     HasPlayedOldGame = Symbol(
         [0x4CA70],
         [0x204CA70],
         None,
         "Returns the value of the VAR_PLAY_OLD_GAME script variable.\n\nreturn: bool",
     )
 
@@ -3775,21 +3899,21 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: dungeon ID\nr1:"
             " bit_value"
         ),
     )
 
-    CheckDungeonOpen = Symbol(
+    GetDungeonMode = Symbol(
         [0x4CF9C],
         [0x204CF9C],
         None,
         (
-            "Related to dungeon open list\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: dungeon ID\nreturn: status code?"
+            "Returns the mode of the specified dungeon\n\nr0: Dungeon ID\nreturn:"
+            " Dungeon mode"
         ),
     )
 
     GlobalProgressAlloc = Symbol(
         [0x4D108],
         [0x204D108],
         None,
@@ -4002,14 +4126,59 @@
         (
             "If buffer_portrait is null, it only checks if it exists\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: portrait box pointer\nr1:"
             " buffer_portrait\nreturn: exists"
         ),
     )
 
+    SetEnterDungeon = Symbol(
+        [0x4E94C],
+        [0x204E94C],
+        None,
+        (
+            "Used to set the dungeon that will be accessed when switching from ground"
+            " to dungeon mode.\n\nr0: Dungeon ID"
+        ),
+    )
+
+    InitDungeonInit = Symbol(
+        [0x4EA5C],
+        [0x204EA5C],
+        None,
+        (
+            "Initializes the dungeon_init struct before entering a dungeon.\n\nr0:"
+            " [output] Pointer to the struct to init\nr1: Dungeon ID"
+        ),
+    )
+
+    IsNoLossPenaltyDungeon = Symbol(
+        [0x4EFE0],
+        [0x204EFE0],
+        None,
+        (
+            "Returns true if the specified dungeon shouldn't have a loss penalty.\n\nIf"
+            " true you won't lose your money and items upon fainting. Also used to"
+            " initialize dungeon_init::skip_faint_animation_flag.\n\nReturns: True for"
+            " DUNGEON_CRYSTAL_LAKE and DUNGEON_5TH_STATION_CLEARING, as well as for"
+            " DUNGEON_DEEP_STAR_CAVE_TEAM_ROGUE if the ground variable SIDE01_BOSS2ND"
+            " is 0; false otherwise."
+        ),
+    )
+
+    CheckMissionRestrictions = Symbol(
+        [0x4F3C4],
+        [0x204F3C4],
+        None,
+        (
+            "Seems to be used to check if you have any missions that have unmet"
+            " restrictions when trying to access a dungeon.\n\nr0: ?\nreturn: (?) Seems"
+            " to be composed of multiple bitflags."
+        ),
+    )
+
     GetNbFloors = Symbol(
         [0x4F57C],
         [0x204F57C],
         None,
         (
             "Returns the number of floors of the given dungeon.\n\nThe result is"
             " hardcoded for certain dungeons, such as dojo mazes.\n\nr0: Dungeon"
@@ -4071,19 +4240,75 @@
         (
             "Given a dungeon ID and a floor number, returns a struct with the"
             " corresponding dungeon group and floor number in that group.\n\nThe"
             " function normally uses the data in mappa_s.bin to calculate the result,"
             " but there's some dungeons (such as dojo mazes) that have hardcoded return"
             " values.\n\nIrdkwia's notes:\n  [r1]: dungeon_id\n  [r1+1]:"
             " dungeon_floor_id\n  [r0]: group_id\n  [r0+1]: group_floor_id\n\nr0:"
-            " (output) Struct containing the dungeon group and floor group\nr1: Struct"
+            " [output] Struct containing the dungeon group and floor group\nr1: Struct"
             " containing the dungeon ID and floor number"
         ),
     )
 
+    GetMissionRank = Symbol(
+        [0x4F814],
+        [0x204F814],
+        None,
+        (
+            "Gets the mission rank for the given dungeon and floor.\n\nIf the dungeon"
+            " ID is >= DUNGEON_NORMAL_FLY_MAZE or the group of the dungeon is >"
+            " DGROUP_DUMMY_0x63, returns MISSION_RANK_E.\n\nr0: Dungeon and"
+            " floor\nreturn: Mission rank"
+        ),
+    )
+
+    GetOutlawLevel = Symbol(
+        [0x4F88C],
+        [0x204F88C],
+        None,
+        (
+            "Gets the level that should be used for outlaws for the given dungeon and"
+            " floor\n\nr0: Dungeon and floor\nreturn: Outlaw level"
+        ),
+    )
+
+    GetOutlawLeaderLevel = Symbol(
+        [0x4F8A8],
+        [0x204F8A8],
+        None,
+        (
+            "Gets the level that should be used for team leader outlaws for the given"
+            " dungeon and floor. Identical to GetOutlawLevel.\n\nr0: Dungeon and"
+            " floor\nreturn: Outlaw leader level"
+        ),
+    )
+
+    GetOutlawMinionLevel = Symbol(
+        [0x4F8C4],
+        [0x204F8C4],
+        None,
+        (
+            "Gets the level that should be used for minion outlaws for the given"
+            " dungeon and floor.\n\nr0: Dungeon and floor\nreturn: Outlaw minion level"
+        ),
+    )
+
+    AddGuestMonster = Symbol(
+        [0x4F8E0],
+        [0x204F8E0],
+        None,
+        (
+            "Adds a guest monster to the active team\n\nr0: dungeon_init struct for the"
+            " dungeon that is about to be entered\nr1: Number of the guest monster to"
+            " add. Used when more than one monster is added.\nr2: Pointer to the guest"
+            " monster entry to add to the team (usually located within"
+            " GUEST_MONSTER_DATA)"
+        ),
+    )
+
     GetGroundNameId = Symbol(
         [0x4F958], [0x204F958], None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetAdventureLogStructLocation = Symbol(
         [0x4FA24],
         [0x204FA24],
@@ -5181,14 +5406,24 @@
     LoadM2nAndN2m = Symbol(
         [0x52BD4],
         [0x2052BD4],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    GuestMonsterToGroundMonster = Symbol(
+        [0x52E50],
+        [0x2052E50],
+        None,
+        (
+            "Inits a ground_monster entry with the given guest_monster struct.\n\nr0:"
+            " [output] ground_monster struct to init\nr1: guest_monster struct to use"
+        ),
+    )
+
     StrcmpMonsterName = Symbol(
         [0x52FB0],
         [0x2052FB0],
         None,
         (
             "Checks if the string_buffer matches the name of the species\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: string_buffer\nr1: monster"
@@ -5760,15 +5995,15 @@
         [0x58D04],
         [0x2058D04],
         None,
         (
             "Determines the list of IQ skills that a given monster can learn given its"
             " IQ value.\n\nThe list of skills is written in the array specified in r0."
             " The array has 69 slots in total. Unused slots are set to 0.\n\nr0:"
-            " (output) Array where the list of skills will be written\nr1: Monster"
+            " [output] Array where the list of skills will be written\nr1: Monster"
             " species\nr2: Monster IQ\nreturn: Amount of skills written to the output"
             " array"
         ),
     )
 
     DisableIqSkill = Symbol(
         [0x58DA4],
@@ -6215,14 +6450,29 @@
         (
             "Converts an index in DUNGEON_SWAP_ID_TABLE to the corresponding dungeon"
             " ID, or DUNGEON_DUMMY_0xFF if the index is -1.\n\nr0: index\nreturn:"
             " dungeon ID"
         ),
     )
 
+    GetDungeonModeSpecial = Symbol(
+        [0x6A76C],
+        [0x206A76C],
+        None,
+        (
+            "Returns the status of the given dungeon, with some modifications.\n\nIf"
+            " the dungeon ID is DUNGEON_BEACH, returns DMODE_REQUEST.\nIf it's"
+            " DUNGEON_JOINED_AT_UNKNOWN, returns DMODE_OPEN_AND_REQUEST.\nIf it's >="
+            " DUNGEON_NORMAL_FLY_MAZE and <= DUNGEON_DOJO_0xD3, returns"
+            " DMODE_OPEN_AND_REQUEST.\nElse, calls GetDungeonMode and returns"
+            " DMODE_REQUEST if the dungeon has been cleared, or DMODE_OPEN if it's"
+            " not.\n\nr0: Dungeon ID\nreturn: Dungeon mode"
+        ),
+    )
+
     ResumeBgm = Symbol(
         [0x6D9BC],
         [0x206D9BC],
         None,
         "Uncertain.\n\nNote: unverified, ported from Irdkwia's notes",
     )
 
@@ -6233,14 +6483,94 @@
     UpdateChannels = Symbol(
         [0x7448C],
         [0x207448C],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nNo params.",
     )
 
+    ClearIrqFlag = Symbol(
+        [0x7B7D0],
+        [0x207B7D0],
+        None,
+        (
+            "Enables processor interrupts by clearing the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were disabled, 0x0 if they were already enabled)"
+        ),
+    )
+
+    EnableIrqFlag = Symbol(
+        [0x7B7E4],
+        [0x207B7E4],
+        None,
+        (
+            "Disables processor interrupts by setting the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were already disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    SetIrqFlag = Symbol(
+        [0x7B7F8],
+        [0x207B7F8],
+        None,
+        (
+            "Sets the value of the processor's interrupt flag according to the"
+            " specified parameter.\n\nr0: Value to set the flag to (0x80 to set it,"
+            " which disables interrupts; 0x0 to unset it, which enables"
+            " interrupts)\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts were"
+            " disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    EnableIrqFiqFlags = Symbol(
+        [0x7B810],
+        [0x207B810],
+        None,
+        (
+            "Disables processor all interrupts (both standard and fast) by setting the"
+            " i and f flags in the program status register (cpsr).\n\nreturn: Old value"
+            " of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    SetIrqFiqFlags = Symbol(
+        [0x7B824],
+        [0x207B824],
+        None,
+        (
+            "Sets the value of the processor's interrupt flags (i and f) according to"
+            " the specified parameter.\n\nr0: Value to set the flags to (0xC0 to set"
+            " both flags, 0x80 to set the i flag and clear the f flag, 0x40 to set the"
+            " f flag and clear the i flag and 0x0 to clear both flags)\nreturn: Old"
+            " value of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    GetIrqFlag = Symbol(
+        [0x7B83C],
+        [0x207B83C],
+        None,
+        (
+            "Gets the current value of the processor's interrupt request (i)"
+            " flag\n\nreturn: cpsr & 0x80 (0x80 if interrupts are disabled, 0x0 if they"
+            " are enabled)"
+        ),
+    )
+
+    WaitForever2 = Symbol(
+        [0x7BC20],
+        [0x207BC20],
+        None,
+        (
+            "Calls EnableIrqFlag and WaitForInterrupt in an infinite loop.\n\nThis is"
+            " called on fatal errors to hang the program indefinitely.\n\nNo params."
+        ),
+    )
+
     WaitForInterrupt = Symbol(
         [0x7BC30],
         [0x207BC30],
         None,
         (
             "Presumably blocks until the program receives an interrupt.\n\nThis just"
             " calls (in Ghidra terminology) coproc_moveto_Wait_for_interrupt(0). See"
@@ -12967,14 +13297,24 @@
         0x4,
         (
             "The multiplier for damage from the Air Blade (1.5), as a binary"
             " fixed-point number (8 fraction bits)"
         ),
     )
 
+    KECLEON_SHOP_BOOST_CHANCE_MULTIPLIER = Symbol(
+        [0x7DCC],
+        [0x22C484C],
+        0x4,
+        (
+            "The boosted kecleon shop spawn chance multiplier (~1.2) as a binary"
+            " fixed-point number (8 fraction bits)."
+        ),
+    )
+
     HIDDEN_STAIRS_SPAWN_CHANCE_MULTIPLIER = Symbol(
         [0x7DD0],
         [0x22C4850],
         0x4,
         (
             "The hidden stairs spawn chance multiplier (~1.2) as a binary fixed-point"
             " number (8 fraction bits), if applicable. See"
@@ -13655,16 +13995,18 @@
     )
 
     LoadBackgroundAttributes = Symbol(
         [0xF900],
         [0x22EBB40],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: [output]"
-            " bg_attr_str\nr1: bg_id"
+            "Open and read an entry from the MAP_BG/bg_list.dat\n\nDocumentation on"
+            " this format can be found"
+            " here:\nhttps://github.com/SkyTemple/skytemple-files/tree/55b3017631a8a1b0f106111ef91a901dc394c6df/skytemple_files/graphics/bg_list_dat\n\nr0:"
+            " [output] The entry\nr1: background ID"
         ),
     )
 
     LoadMapType10 = Symbol(
         [0x10AE4],
         [0x22ECD24],
         None,
@@ -13767,14 +14109,24 @@
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
             " characters printed, excluding the null-terminator"
         ),
     )
 
+    GetExclusiveItemRequirements = Symbol(
+        [0x2ECF8],
+        [0x230AF38],
+        None,
+        (
+            "Used to calculate the items required to get a certain exclusive item in"
+            " the swap shop.\n\nr0: ?\nr1: ?"
+        ),
+    )
+
     StatusUpdate = Symbol(
         [0x37858],
         [0x2313A98],
         None,
         (
             "Implements SPECIAL_PROC_STATUS_UPDATE (see"
             " ScriptSpecialProcessCall).\n\nNo params."
@@ -13933,14 +14285,18 @@
         ),
     )
 
     UNIONALL_RAM_ADDRESS = Symbol([0x48A64], [0x2324CA4], None, "[Runtime]")
 
     GROUND_STATE_MAP = Symbol([0x48A80], [0x2324CC0], None, "[Runtime]")
 
+    GROUND_STATE_WEATHER = Symbol(
+        None, None, None, "[Runtime] Same structure format as GROUND_STATE_MAP"
+    )
+
     GROUND_STATE_PTRS = Symbol(
         [0x48AB4],
         [0x2324CF4],
         0x18,
         (
             "Host pointers to multiple structure used for performing an overworld"
             " scene\n\ntype: struct main_ground_data"
@@ -15930,24 +16286,81 @@
     FadeToBlack = Symbol(
         [0x4728],
         [0x22E0968],
         None,
         "Fades the screen to black across several frames.\n\nNo params.",
     )
 
+    CheckTouchscreenArea = Symbol(
+        [0x4A78],
+        [0x22E0CB8],
+        None,
+        (
+            "Checks if the currently pressed touchscreen position is within the"
+            " specified area.\n\nr0: Area lower X coordinate\nr1: Area lower Y"
+            " coordinate\nr2: Area upper X coordinate\nr3: Area upper Y"
+            " coordinate\nreturn: True if the specified area contains the currently"
+            " pressed touchscreen position, false otherwise."
+        ),
+    )
+
+    GetTrapInfo = Symbol(
+        [0x53C8],
+        [0x22E1608],
+        None,
+        (
+            "Given a trap entity, returns the pointer to the trap info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Trap data pointer"
+        ),
+    )
+
+    GetItemInfo = Symbol(
+        [0x53D0],
+        [0x22E1610],
+        None,
+        (
+            "Given an item entity, returns the pointer to the item info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Item data pointer"
+        ),
+    )
+
     GetTileAtEntity = Symbol(
         [0x53E8],
         [0x22E1628],
         None,
         (
             "Returns a pointer to the tile where an entity is located.\n\nr0: pointer"
             " to entity\nreturns: pointer to tile"
         ),
     )
 
+    UpdateEntityPixelPos = Symbol(
+        [0x5800],
+        [0x22E1A40],
+        None,
+        (
+            "Updates an entity's pixel_pos field using the specified pixel_position"
+            " struct, or its own pos field if it's null.\n\nr0: Entity pointer\nr1:"
+            " Pixel position to use, or null to use the entity's own position"
+        ),
+    )
+
+    CreateEnemyEntity = Symbol(
+        [0x5E80],
+        [0x22E20C0],
+        None,
+        (
+            "Creates and initializes the entity struct of a newly spawned enemy"
+            " monster. Fails if there's 16 enemies on the floor already.\n\nIt could"
+            " also be used to spawn fixed room allies, since those share their slots on"
+            " the entity list.\n\nr0: Monster ID\nreturn: Pointer to the newly"
+            " initialized entity, or null if the entity couldn't be initialized"
+        ),
+    )
+
     SpawnTrap = Symbol(
         [0x6020],
         [0x22E2260],
         None,
         (
             "Spawns a trap on the floor. Fails if there are more than 64 traps already"
             " on the floor.\n\nThis modifies the appropriate fields on the dungeon"
@@ -15967,35 +16380,46 @@
             " items already on the floor.\n\nThis initializes a new entry in the entity"
             " table and points it to the corresponding slot in the item info"
             " list.\n\nr0: position\nreturn: entity pointer for the newly added item,"
             " or null on failure"
         ),
     )
 
-    ShouldDisplayEntityMessages = Symbol(
+    ShouldMinimapDisplayEntity = Symbol(
+        [0x6258],
+        [0x22E2498],
+        None,
+        (
+            "Checks if a given entity should be displayed on the minimap\n\nr0: Entity"
+            " pointer\nreturn: True if the entity should be displayed on the minimap"
+        ),
+    )
+
+    ShouldDisplayEntity = Symbol(
         [0x6334],
         [0x22E2574],
         None,
         (
-            "Checks if messages that involve a certain entity should be displayed or"
-            " suppressed.\n\nFor example, it returns false if the entity is an"
-            " invisible enemy.\n\nr0: Entity pointer\nr1: ?\nreturn: True if messages"
-            " involving the entity should be displayed, false if they should be"
-            " suppressed."
+            "Checks if an entity should be displayed or not.\n\nFor example, it returns"
+            " false if the entity is an invisible enemy.\nAlso used to determine if"
+            " messages that involve a certain entity should be displayed or"
+            " suppressed.\n\nr0: Entity pointer\nr1: (?) Seems to be 1 for monsters and"
+            " 0 for items.\nreturn: True if the entity and its associated messages"
+            " should be displayed, false if they shouldn't."
         ),
     )
 
-    ShouldDisplayEntityMessagesWrapper = Symbol(
+    ShouldDisplayEntityWrapper = Symbol(
         [0x64EC],
         [0x22E272C],
         None,
         (
-            "Calls ShouldDisplayEntityMessages with r1 = 0\n\nr0: Entity"
-            " pointer\nreturn: True if messages involving the entity should be"
-            " displayed, false if they should be suppressed."
+            "Calls ShouldDisplayEntity with r1 = 0\n\nr0: Entity pointer\nreturn: True"
+            " if the entity and its associated messages should be displayed, false if"
+            " they shouldn't."
         ),
     )
 
     CanSeeTarget = Symbol(
         [0x650C],
         [0x22E274C],
         None,
@@ -16143,28 +16567,54 @@
         (
             "Returns dungeon::display_data::visibility_range. If the visibility range"
             " is 0, returns 2 instead.\n\nreturn: Visibility range of the current"
             " floor, or 2 if the visibility is 0."
         ),
     )
 
-    PlayEffectAnimation = Symbol(
+    PlayEffectAnimationEntity = Symbol(
         [0x73A4],
         [0x22E35E4],
         None,
         (
             "Just a guess. This appears to be paired often with"
             " GetEffectAnimationField0x19, and also has calls AnimationHasMoreFrames in"
             " a loop alongside AdvanceFrame(66) calls.\n\nThe third parameter skips the"
             " loop entirely. It seems like in this case the function might just preload"
-            " some animation frames for later use??\n\nr0: entity pointer\nr1: ?\nr2:"
-            " appears to be a flag for actually running the animation now? If this is"
-            " 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn: status"
-            " code, or maybe the number of frames or something? Either way, -1 seems to"
-            " indicate the animation being finished or something?"
+            " some animation frames for later use??\n\nr0: entity pointer\nr1: Effect"
+            " ID\nr2: appears to be a flag for actually running the animation now? If"
+            " this is 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn:"
+            " status code, or maybe the number of frames or something? Either way, -1"
+            " seems to indicate the animation being finished or something?"
+        ),
+    )
+
+    PlayEffectAnimationPos = Symbol(
+        [0x759C],
+        [0x22E37DC],
+        None,
+        (
+            "Takes a position struct in r0 and converts it to a pixel position struct"
+            " before calling PlayEffectAnimationPixelPos\n\nr0: Position where the"
+            " effect should be played\nr1: Effect ID\nr2: Unknown flag (same as the one"
+            " in PlayEffectAnimationEntity)\nreturn: Result of call to"
+            " PlayEffectAnimationPixelPos"
+        ),
+    )
+
+    PlayEffectAnimationPixelPos = Symbol(
+        [0x75E0],
+        [0x22E3820],
+        None,
+        (
+            "Seems like a variant of PlayEffectAnimationEntity that uses pixel"
+            " coordinates as its first parameter instead of an entity pointer.\n\nr0:"
+            " Pixel position where the effect should be played\nr1: Effect ID\nr2:"
+            " Unknown flag (same as the one in PlayEffectAnimationEntity)\nreturn: Same"
+            " as PlayEffectAnimationEntity"
         ),
     )
 
     UpdateStatusIconFlags = Symbol(
         [0x7874],
         [0x22E3AB4],
         None,
@@ -16252,15 +16702,15 @@
         [0x22E7C60],
         None,
         (
             "Copies all entries in the floor's monster spawn list that have a sprite"
             " size >= 6 to the specified buffer.\n\nThe parameter in r1 can be used to"
             " specify how many entries are already present in the buffer. Entries added"
             " by this function will be placed after those, and the total returned in r1"
-            " will account for existing entries as well.\n\nr0: (output) Buffer where"
+            " will account for existing entries as well.\n\nr0: [output] Buffer where"
             " the result will be stored\nr1: Current amount of entries in the"
             " buffer\nreturn: New amount of entries in the buffer"
         ),
     )
 
     IsOnMonsterSpawnList = Symbol(
         [0xBB0C],
@@ -16632,14 +17082,26 @@
             " the effect of the Switcher Orb). \n\nThe function checks for the Suction"
             " Cups ability for both the user and the target, and for the Mold Breaker"
             " ability on the user.\n\nr0: pointer to user entity\nr1: pointer to target"
             " entity"
         ),
     )
 
+    SetLeaderActionFields = Symbol(
+        [0xF188],
+        [0x22EB3C8],
+        None,
+        (
+            "Sets the leader's monster::action::action_id to the specified"
+            " value.\n\nAlso sets monster::action::action_use_idx and"
+            " monster::action::field_0xA to 0, as well as monster::action::field_0x10"
+            " and monster::action::field_0x12 to -1.\n\nr0: ID of the action to set"
+        ),
+    )
+
     ClearMonsterActionFields = Symbol(
         [0xF1B4],
         [0x22EB3F4],
         None,
         (
             "Clears the fields related to AI in the monster's data struct, setting them"
             " all to 0.\nSpecifically, monster::action::action_id,"
@@ -16719,14 +17181,27 @@
         (
             "Sets a monster's action to action::ACTION_REGULAR_ATTACK, with a specified"
             " direction.\n\nr0: Pointer to the monster's action field\nr1: Direction in"
             " which to use the move. Gets stored in monster::action::direction."
         ),
     )
 
+    SetActionUseMovePlayer = Symbol(
+        [0xFA58],
+        [0x22EBC98],
+        None,
+        (
+            "Sets a monster's action to action::ACTION_USE_MOVE_PLAYER, with a"
+            " specified monster and move index.\n\nr0: Pointer to the monster's action"
+            " field\nr1: Index of the monster that is using the move on the entity"
+            " list. Gets stored in monster::action::action_use_idx.\nr2: Index of the"
+            " move to use (0-3). Gets stored in monster::action::field_0xA."
+        ),
+    )
+
     SetActionUseMoveAi = Symbol(
         [0xFA7C],
         [0x22EBCBC],
         None,
         (
             "Sets a monster's action to action::ACTION_USE_MOVE_AI, with a specified"
             " direction and move index.\n\nr0: Pointer to the monster's action"
@@ -16873,14 +17348,169 @@
             "If the flag for a trapper trap is set, handles spawning a trap based upon"
             " the\ninformation inside the dungeon struct. Uses the entity for logging a"
             " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
             " true if a trap was spawned succesfully"
         ),
     )
 
+    TryTriggerTrap = Symbol(
+        [0x11D60],
+        [0x22EDFA0],
+        None,
+        (
+            "Called whenever a monster steps on a trap.\n\nThe function will try to"
+            " trigger it. Nothing will happen if the pokémon has the same team as the"
+            " trap. The attempt to trigger the trap can also fail due to IQ skills, due"
+            " to the trap failing to work (random chance), etc.\n\nr0: Entity who"
+            " stepped on the trap\nr1: Trap position\nr2: ?\nr3: ?"
+        ),
+    )
+
+    ApplyMudTrapEffect = Symbol(
+        [0x1212C],
+        [0x22EE36C],
+        None,
+        (
+            "Randomly lowers attack, special attack, defense, or special defense of the"
+            " defender by 3 stages.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer"
+        ),
+    )
+
+    ApplyStickyTrapEffect = Symbol(
+        [0x121F4],
+        [0x22EE434],
+        None,
+        (
+            "If the defender is the leader, randomly try to make something in the bag"
+            " sticky. Otherwise, try to make the item the monster is holding"
+            " sticky.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyGrimyTrapEffect = Symbol(
+        [0x123EC],
+        [0x22EE62C],
+        None,
+        (
+            "If the defender is the leader, randomly try to turn food items in the"
+            " toolbox into\ngrimy food. Otherwise, try to make the food item the"
+            " monster is holding grimy food.\n\nr0: attacker entity pointer\nr1:"
+            " defender entity pointer"
+        ),
+    )
+
+    ApplyPitfallTrapEffect = Symbol(
+        [0x125E0],
+        [0x22EE820],
+        None,
+        (
+            "If the defender is the leader, end the current floor unless it has a"
+            " rescue point.\nOtherwise, make the entity faint and ignore reviver seeds."
+            " If not called by a random\ntrap, break the grate on the pitfall"
+            " trap.\n\nr0: attacker entity pointer\nr1: defender entity pointer\nr2:"
+            " tile pointer\nr3: bool caused by random trap"
+        ),
+    )
+
+    ApplySummonTrapEffect = Symbol(
+        [0x12754],
+        [0x22EE994],
+        None,
+        (
+            "Randomly spawns 2-4 enemy monsters around the position. The entity is only"
+            " used for\nlogging messages.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyPpZeroTrapEffect = Symbol(
+        [0x127F0],
+        [0x22EEA30],
+        None,
+        (
+            "Tries to reduce the PP of one of the defender's moves to 0.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyPokemonTrapEffect = Symbol(
+        [0x128D8],
+        [0x22EEB18],
+        None,
+        (
+            "Turns item in the same room as the tile at the position (usually just the"
+            " entities's\nposition) into monsters. If the position is in a hallway,"
+            " convert items in a 3x3 area\ncentered on the position into"
+            " monsters.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTripTrapEffect = Symbol(
+        [0x12AEC],
+        [0x22EED2C],
+        None,
+        (
+            "Tries to drop the defender's item and places it on the floor.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyToxicSpikesTrapEffect = Symbol(
+        [0x12CAC],
+        [0x22EEEEC],
+        None,
+        (
+            "Tries to inflict 10 damage on the defender and then tries to poison"
+            " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyRandomTrapEffect = Symbol(
+        [0x12D00],
+        [0x22EEF40],
+        None,
+        (
+            "Selects a random trap that isn't a wonder tile and isn't a random trap and"
+            " calls\nApplyTrapEffect on all monsters that is different from the trap's"
+            " team.\n\nr0: Triggered trap\nr1: User\nr2: Target, normally same as"
+            " user\nr3: Tile that contains the trap\nstack[0]: position"
+        ),
+    )
+
+    ApplyGrudgeTrapEffect = Symbol(
+        [0x12E34],
+        [0x22EF074],
+        None,
+        (
+            "Spawns several monsters around the position and gives all monsters on the"
+            " floor the\ngrudge status condition.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTrapEffect = Symbol(
+        [0x12F14],
+        [0x22EF154],
+        None,
+        (
+            "Performs the effect of a triggered trap.\n\nThe trap's animation happens"
+            " before this function is called.\n\nr0: Triggered trap\nr1: User\nr2:"
+            " Target, normally same as user\nr3: Tile that contains the trap\nstack[0]:"
+            " position\nstack[1]: trap ID\nstack[2]: bool caused by random"
+            " trap\nreturn: True if the trap should be destroyed after the effect is"
+            " applied"
+        ),
+    )
+
+    RevealTrapsNearby = Symbol(
+        [0x13398],
+        [0x22EF5D8],
+        None,
+        "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x1382C],
         [0x22EFA6C],
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16904,28 +17534,63 @@
         None,
         (
             "Returns a pointer to the action data of the current leader (field 0x4A on"
             " its monster struct).\n\nNo params."
         ),
     )
 
+    GetEntityTouchscreenArea = Symbol(
+        [0x1496C],
+        [0x22F0BAC],
+        None,
+        (
+            "Returns the area on the touchscreen that contains the sprite of the"
+            " specified entity\n\nr0: Entity pointer\nr1: [output] struct where the"
+            " result should be written"
+        ),
+    )
+
     SetLeaderAction = Symbol(
         [0x14C9C],
         [0x22F0EDC],
         None,
         (
             "Sets the leader's action field depending on the inputs given by the"
             " player.\n\nThis function also accounts for other special situations that"
             " can force a certain action, such as when the leader is running. The"
             " function also takes care of opening the main menu when X is pressed.\nThe"
             " function generally doesn't return until the player has an action"
             " set.\n\nNo params."
         ),
     )
 
+    ShouldLeaderKeepRunning = Symbol(
+        [0x16E4C],
+        [0x22F308C],
+        None,
+        (
+            "Determines if the leader should keep running. Returns false if the leader"
+            " bumps into something, or if an action that should stop the leader takes"
+            " place.\n\nreturn: True if the leader should keep running, false if it"
+            " should stop."
+        ),
+    )
+
+    CheckLeaderTile = Symbol(
+        [0x173F4],
+        [0x22F3634],
+        None,
+        (
+            "Checks the tile the leader just stepped on and performs any required"
+            " actions, such as picking up items, triggering traps, etc.\n\nContains a"
+            " switch that checks the type of the tile the leader just stepped on.\n\nNo"
+            " params."
+        ),
+    )
+
     ChangeLeader = Symbol(
         [0x176F4],
         [0x22F3934],
         None,
         (
             "Tries to change the current leader to the monster specified by"
             " dungeon::new_leader.\n\nAccounts for situations that can prevent changing"
@@ -17068,14 +17733,25 @@
         (
             "Handles a fainted pokémon (reviving does not count as fainting).\n\nr0:"
             " Fainted entity\nr1: Damage source (move ID or greater than the max move"
             " id for other causes)\nr2: Entity responsible of the fainting"
         ),
     )
 
+    MoveMonsterToPos = Symbol(
+        [0x1C3B0],
+        [0x22F85F0],
+        None,
+        (
+            "Moves a monster to the target position. Used both for regular movement and"
+            " special movement (like teleportation).\n\nr0: Entity pointer\nr1: X"
+            " target position\nr2: Y target position\nr3: ?"
+        ),
+    )
+
     UpdateAiTargetPos = Symbol(
         [0x1CF04],
         [0x22F9144],
         None,
         (
             "Given a monster, updates its target_pos field based on its current"
             " position and the direction in which it plans to attack.\n\nr0: Entity"
@@ -17220,14 +17896,24 @@
             "Restores PP for all moves, clears flags move::f_consume_2_pp,"
             " move::flags2_unk5 and move::flags2_unk7, and sets flag"
             " move::f_consume_pp.\nCalled when a monster is revived.\n\nr0: pointer to"
             " entity whose moves will be restored"
         ),
     )
 
+    BoostIQ = Symbol(
+        [0x1DF04],
+        [0x22FA144],
+        None,
+        (
+            "Tries to boost the target's IQ.\n\nr0: monster entity pointer\nr1: iq"
+            " boost\nr2: bool suppress logs"
+        ),
+    )
+
     ShouldMonsterHeadToStairs = Symbol(
         [0x1E1F0],
         [0x22FA430],
         None,
         (
             "Checks if a given monster should try to reach the stairs when controlled"
             " by the AI\n\nr0: Entity pointer\nreturn: True if the monster should try"
@@ -17244,14 +17930,28 @@
             " dungeon::mew_cannot_spawn or the second parameter are true.\n\nCalled"
             " before spawning an enemy, appears to be checking if Mew can spawn on the"
             " current floor.\n\nr0: monster id\nr1: return false if the monster id is"
             " Mew\nreturn: bool"
         ),
     )
 
+    TryEndStatusWithAbility = Symbol(
+        [0x1E59C],
+        [0x22FA7DC],
+        None,
+        (
+            "Checks if any of the defender's active abilities would end one of their"
+            " current status\nconditions. For example, if the ability Own Tempo will"
+            " stop confusion.\n\nCalled after changing a monster's ability with skill"
+            " swap, role play, or trace to\nremove statuses the monster should no"
+            " longer be affected by.\n\nr0: attacker entity pointer\nr1: defender"
+            " entity pointer"
+        ),
+    )
+
     ExclusiveItemEffectIsActive = Symbol(
         [
             0x1EA58,
             0x23CE8,
             0x2E778,
             0x3366C,
             0x34E24,
@@ -17407,14 +18107,27 @@
             "Checks if a monster does not gain experience.\n\nThis basically just"
             " inverts IsSpecialStoryAlly, with the exception of also checking for the"
             " 'Joined At' field being DUNGEON_CLIENT (is this set for mission"
             " clients?).\n\nr0: monster pointer\nreturn: bool"
         ),
     )
 
+    InitOtherMonsterData = Symbol(
+        [0x1FC18],
+        [0x22FBE58],
+        None,
+        (
+            "Initializes stats, IQ skills and moves for a given monster\n\nMight only"
+            " be used when spawning fixed room monsters.\n\nr0: Entity pointer\nr1:"
+            " Fixed room monster stats index\nr2: Spawn direction? (when calling this"
+            " function while spawning a fixed room monster, this is the parameter value"
+            " associated to the spawn action, after converting it to a direction.)"
+        ),
+    )
+
     SpawnTeam = Symbol(
         [0x202CC],
         [0x22FC50C],
         None,
         "Seems to initialize and spawn the team when entering a dungeon.\n\nr0: ?",
     )
 
@@ -17454,20 +18167,32 @@
             " to the struct containing the data of the team member to"
             " initialize\nstack[0]: ?\nstack[1]: ?\nstack[2]: ?\nstack[3]:"
             " ?\nstack[4]: ?"
         ),
     )
 
     InitMonster = Symbol(
+        [0x21794],
+        [0x22FD9D4],
+        None,
+        (
+            "Initializes the monster struct within the provided entity struct.\n\nr0:"
+            " ?\nr1: Pointer to the entity whose monster struct should be"
+            " initialized\nr2: pointer to the entity's spawned_monster_data struct\nr3:"
+            " (?) Pointer to something"
+        ),
+    )
+
+    SubInitMonster = Symbol(
         [0x21B80],
         [0x22FDDC0],
         None,
         (
-            "Initializes a monster struct.\n\nr0: pointer to monster to initialize\nr1:"
-            " some flag"
+            "Called by InitMonster. Initializes some fields on the monster"
+            " struct.\n\nr0: pointer to monster to initialize\nr1: some flag"
         ),
     )
 
     MarkShopkeeperSpawn = Symbol(
         [0x21F58],
         [0x22FE198],
         None,
@@ -17572,14 +18297,24 @@
         (
             "Returns the number of attacks that a monster can do in one turn (1 or"
             " 2).\n\nChecks for the abilities Swift Swim, Chlorophyll, Unburden, and"
             " for exclusive items.\n\nr0: pointer to entity\nreturns: int"
         ),
     )
 
+    GetMonsterDisplayNameType = Symbol(
+        [0x23EC8],
+        [0x2300108],
+        None,
+        (
+            "Determines how the name of a monster should be displayed.\n\nr0: Entity"
+            " pointer\nreturn: Display name type"
+        ),
+    )
+
     GetMonsterName = Symbol(
         [0x23F24],
         [0x2300164],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: buffer\nr1: TargetInfo",
     )
 
@@ -17730,14 +18465,39 @@
         None,
         (
             "Checks if a monster has the sleep, nightmare, or napping status.\n\nr0:"
             " entity pointer\nreturn: bool"
         ),
     )
 
+    CanMonsterMoveInDirection = Symbol(
+        [0x24E1C],
+        [0x230105C],
+        None,
+        (
+            "Checks if the given monster can move in the specified direction\n\nReturns"
+            " false if any monster is standing on the target tile\n\nr0: Monster entity"
+            " pointer\nr1: Direction to check\nreturn: bool"
+        ),
+    )
+
+    GetFinalMobilityType = Symbol(
+        [0x24CF0],
+        [0x2300F30],
+        None,
+        (
+            "Returns the mobility type of a monster, after accounting for things that"
+            " could affect it (like items or IQ skills)\n\nIf the specified direction"
+            " is DIR_NONE, direction checks are skipped. If it's not,"
+            " MOBILITY_INTANGIBLE is only returned if the direction is not"
+            " diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility type\nr2:"
+            " Direction of mobility\nreturn: Final mobility type"
+        ),
+    )
+
     IsMonsterCornered = Symbol(
         [0x24ED8],
         [0x2301118],
         None,
         (
             "True if the given monster is cornered (it can't move in any"
             " direction)\n\nr0: Entity pointer\nreturn: True if the monster can't move"
@@ -17765,15 +18525,15 @@
         [0x23012F8],
         None,
         (
             "Checks whether an AI-controlled monster can move in the specified"
             " direction.\nAccounts for walls, other monsters on the target position and"
             " IQ skills that might prevent a monster from moving into a specific"
             " location, such as House Avoider, Trap Avoider or Lava Evader.\n\nr0:"
-            " Entity pointer\nr1: Direction\nr2: (output) True if movement was not"
+            " Entity pointer\nr1: Direction\nr2: [output] True if movement was not"
             " possible because there was another monster on the target tile, false"
             " otherwise.\nreturn: True if the monster can move in the specified"
             " direction, false otherwise."
         ),
     )
 
     ShouldMonsterRunAway = Symbol(
@@ -17793,14 +18553,47 @@
         (
             "Calls ShouldMonsterRunAway and returns its result. It also calls another"
             " function if the result was true.\n\nr0: Entity pointer\nr1: ?\nreturn:"
             " Result of the call to ShouldMonsterRunAway"
         ),
     )
 
+    SafeguardIsActive = Symbol(
+        [0x25700],
+        [0x2301940],
+        None,
+        (
+            "Checks if the monster is under the effect of Safeguard.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: flag to log a message\nreturn:"
+            " bool"
+        ),
+    )
+
+    LeafGuardIsActive = Symbol(
+        [0x25754],
+        [0x2301994],
+        None,
+        (
+            "Checks if the monster is protected by the ability Leaf Guard.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer\nr2: flag to log a"
+            " message\nreturn: bool"
+        ),
+    )
+
+    IsProtectedFromStatDrops = Symbol(
+        [0x258EC],
+        [0x2301B2C],
+        None,
+        (
+            "Checks if the target monster is protected from getting their stats dropped"
+            " by the user.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     NoGastroAcidStatus = Symbol(
         [0x25A9C],
         [0x2301CDC],
         None,
         (
             "Checks if a monster does not have the Gastro Acid status.\n\nr0: entity"
             " pointer\nreturn: bool"
@@ -17961,14 +18754,25 @@
             "Updates monster::state_flags and monster::prev_state_flags with new"
             " values.\n\nr0: monster pointer\nr1: bitmask for bits to update\nr2:"
             " whether to set the bits indicated by the mask to 1 or 0\nreturn: whether"
             " or not any of the masked bits changed from the previous state"
         ),
     )
 
+    IsProtectedFromNegativeStatus = Symbol(
+        [0x261F0],
+        [0x2302430],
+        None,
+        (
+            "Checks if the target monster is protected from getting a negative status"
+            " condition.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     AddExpSpecial = Symbol(
         [0x262FC],
         [0x230253C],
         None,
         (
             "Adds to a monster's experience points, subject to experience boosting"
             " effects.\n\nThis function appears to be called only under special"
@@ -17982,17 +18786,31 @@
     )
 
     EnemyEvolution = Symbol(
         [0x264BC],
         [0x23026FC],
         None,
         (
-            "Checks if the specified enemy should evolve because it just defeated an"
-            " ally, and if so, attempts to evolve it.\n\nr0: Pointer to the enemy to"
-            " check"
+            "Checks if any enemies on the floor should evolve and attempts to evolve"
+            " it. The\nentity pointer passed seems to get replaced by a generic"
+            " placeholder entity if the\nentity pointer passed is invalid.\n\nr0:"
+            " entity pointer"
+        ),
+    )
+
+    LevelUpItemEffect = Symbol(
+        [0x2681C],
+        [0x2302A5C],
+        None,
+        (
+            "Attempts to level up the the target. Calls LevelUp with a few extra checks"
+            " and messages\nfor using as an item. Used for the Joy Seed and Golden"
+            " Seed.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: number"
+            " of levels\nr3: bool message flag?\nstack[0]: bool show level up dialog"
+            " (for example 'Hey, I leveled up!' with a portrait)?"
         ),
     )
 
     TryDecreaseLevel = Symbol(
         [0x26D48],
         [0x2302F88],
         None,
@@ -18004,27 +18822,31 @@
     )
 
     LevelUp = Symbol(
         [0x26DFC],
         [0x230303C],
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: user entity"
-            " pointer\nr1: target entity pointer\nr2: message flag?\nr3: ?\nreturn:"
-            " success flag?"
+            "Attempts to level up the the target. Fails if the target's level can't be"
+            " raised. The show show level up dialog bool does nothing for monsters not"
+            " on the team.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " bool message flag?\nr3: bool show level up dialog (for example 'Hey, I"
+            " leveled up!' with a portrait)?\nreturn: success flag"
         ),
     )
 
     EvolveMonster = Symbol(
         [0x27A3C],
         [0x2303C7C],
         None,
         (
-            "Makes the specified monster evolve into the specified species.\n\nr0:"
-            " Pointer to the entity to evolve\nr1: ?\nr2: Species to evolve into"
+            "Makes the specified monster evolve into the specified species. Has a"
+            " special case when\na monster evolves into Ninjask and tries to spawn a"
+            " Shedinja as well.\n\nr0: user entity pointer?\nr1: target pointer to the"
+            " entity to evolve\nr2: Species to evolve into"
         ),
     )
 
     GetSleepAnimationId = Symbol(
         [0x28874],
         [0x2304AB4],
         None,
@@ -18046,14 +18868,58 @@
             " example, this delayed display system is used to display multiple monsters"
             " moving at once even though they take turns sequentially.\n\nr0: Pointer"
             " to an entity. Can be null.\nreturns: Seems to be true if there were any"
             " pending actions to display."
         ),
     )
 
+    CheckNonLeaderTile = Symbol(
+        [0x29454],
+        [0x2305694],
+        None,
+        (
+            "Similar to CheckLeaderTile, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: Entity pointer"
+        ),
+    )
+
+    EndNegativeStatusCondition = Symbol(
+        [0x29684],
+        [0x23058C4],
+        None,
+        (
+            "Cures the target's negative status conditions. The game rarely (if not"
+            " never) calls\nthis function with the bool to remove the wrapping status"
+            " false.\n\nr0: pointer to user\nr1: pointer to target\nr2: bool play"
+            " animation\nr3: bool log failure message\nstack[0]: bool remove wrapping"
+            " status\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    EndNegativeStatusConditionWrapper = Symbol(
+        [0x299E8],
+        [0x2305C28],
+        None,
+        (
+            "Calls EndNegativeStatusCondition with remove wrapping status false.\n\nr0:"
+            " pointer to user\nr1: pointer to target\nr2: bool play animation\nr3: bool"
+            " log failure message\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    TransferNegativeStatusCondition = Symbol(
+        [0x299FC],
+        [0x2305C3C],
+        None,
+        (
+            "Transfers all negative status conditions the user has and gives then to"
+            " the target.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     EndSleepClassStatus = Symbol(
         [0x29D9C],
         [0x2305FDC],
         None,
         (
             "Cures the target's sleep, sleepless, nightmare, yawn or napping status due"
             " to the action of the user, and prints the event to the log.\n\nr0:"
@@ -18159,14 +19025,25 @@
         (
             "Removes the target's magnet rise status due to the action of the user, and"
             " prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
             " target"
         ),
     )
 
+    TransferNegativeBlinkerClassStatus = Symbol(
+        [0x2B6AC],
+        [0x23078EC],
+        None,
+        (
+            "Tries to transfer the the negative blinker class status conditions from"
+            " the user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer\nreturn: Whether or not the status could be transferred"
+        ),
+    )
+
     TryTriggerMonsterHouse = Symbol(
         [0x2BD0C],
         [0x2307F4C],
         None,
         (
             "Triggers a Monster House for an entity, if the right conditions are"
             " met.\n\nConditions: entity is valid and on the team, the tile is a"
@@ -18594,14 +19471,26 @@
         (
             "Inflicts the Sleep status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
             " number of turns\nr3: flag to log a message on failure"
         ),
     )
 
+    IsProtectedFromSleepClassStatus = Symbol(
+        [0x357A4],
+        [0x23119E4],
+        None,
+        (
+            "Checks if the monster is immune to sleep class status conditions.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nr2: ignore safeguard\nr3:"
+            " ignore other protections (exclusive items + leaf guard)\nstack[0]: flag"
+            " to log a message on failure\nreturn: bool"
+        ),
+    )
+
     TryInflictNightmareStatus = Symbol(
         [0x35A0C],
         [0x2311C4C],
         None,
         (
             "Inflicts the Nightmare status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
@@ -19104,91 +19993,638 @@
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
             " to log a message on failure\nr3: flag to only perform the check for"
             " inflicting without actually inflicting\nreturn: Whether or not the status"
             " could be inflicted"
         ),
     )
 
-    TryInflictDestinyBond = Symbol(
+    TryInflictDestinyBondStatus = Symbol(
         [0x39810],
         [0x2315A50],
         None,
         (
             "Inflicts the Destiny Bond status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
-    TryInvisify = Symbol(
+    TryInflictSureShotStatus = Symbol(
+        [0x39930],
+        [0x2315B70],
+        None,
+        (
+            "Inflicts the Sure Shot status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWhifferStatus = Symbol(
+        [0x399C0],
+        [0x2315C00],
+        None,
+        (
+            "Inflicts the Whiffer status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSetDamageStatus = Symbol(
+        [0x39AA8],
+        [0x2315CE8],
+        None,
+        (
+            "Inflicts the Set Damage status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictFocusEnergyStatus = Symbol(
+        [0x39B44],
+        [0x2315D84],
+        None,
+        (
+            "Inflicts the Focus Energy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictDecoyStatus = Symbol(
+        [0x39BE4],
+        [0x2315E24],
+        None,
+        (
+            "Inflicts the Decoy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictCurseStatus = Symbol(
+        [0x39E9C],
+        [0x23160DC],
+        None,
+        (
+            "Inflicts the Curse status condition on a target monster if possible and if"
+            " the user is\na ghost type. Otherwise, just boost the user's defense and"
+            " attack then lower the user's\nspeed.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
+    TryInflictSnatchStatus = Symbol(
+        [0x3A040],
+        [0x2316280],
+        None,
+        (
+            "Inflicts the Snatch status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictTauntStatus = Symbol(
+        [0x3A168],
+        [0x23163A8],
+        None,
+        (
+            "Inflicts the Taunt status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictStockpileStatus = Symbol(
+        [0x3A298],
+        [0x23164D8],
+        None,
+        (
+            "Inflicts the Stockpile condition on a target monster if possible. Won't"
+            " boost the level\nof stockpiling above 3.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nreturn: Whether or not the status could be"
+            " inflicted or boosted"
+        ),
+    )
+
+    TryInflictInvisibleStatus = Symbol(
         [0x3A33C],
         [0x231657C],
         None,
         (
             "Attempts to turn the target invisible.\n\nThe user pointer is only used"
             " when calling LogMessage functions.\n\nr0: user entity pointer\nr1: target"
             " entity pointer"
         ),
     )
 
+    TryInflictPerishSongStatus = Symbol(
+        [0x3A3EC],
+        [0x231662C],
+        None,
+        (
+            "Inflicts the Perish Song status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEncoreStatus = Symbol(
+        [0x3A4E0],
+        [0x2316720],
+        None,
+        (
+            "Inflicts the Encore status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryDecreaseBelly = Symbol(
+        [0x3A698],
+        [0x23168D8],
+        None,
+        (
+            "Tries to reduce the belly size of the target. Only when max belly shrink"
+            " is 0, the\ncurrent belly is reduced by belly to lose. If both are"
+            " non-zero, only the max belly\nshrink is applied.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: belly to lose\nr3: max belly"
+            " shrink"
+        ),
+    )
+
+    TryIncreaseBelly = Symbol(
+        [0x3A970],
+        [0x2316BB0],
+        None,
+        (
+            "Restore belly and possibly boost max belly of the target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " belly to restore\nr3: max belly boost (if belly is full)\nstack[0]: flag"
+            " to log a message"
+        ),
+    )
+
+    TryInflictMuzzledStatus = Symbol(
+        [0x3AEE4],
+        [0x2317124],
+        None,
+        (
+            "Inflicts the Muzzled status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
     TryTransform = Symbol(
         [0x3AFDC],
         [0x231721C],
         None,
         (
             "Attempts to transform the target into the species of a random monster"
             " contained in the list returned by MonsterSpawnListPartialCopy.\n\nThe"
             " user pointer is only used when calling LogMessage functions.\n\nr0: user"
             " entity pointer\nr1: target entity pointer"
         ),
     )
 
+    TryInflictMobileStatus = Symbol(
+        [0x3B1CC],
+        [0x231740C],
+        None,
+        (
+            "Inflicts the Mobile status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictExposedStatus = Symbol(
+        [0x3B288],
+        [0x23174C8],
+        None,
+        (
+            "Inflicts the Exposed status condition on a target monster if possible."
+            " Only applies to\nGhost types and monsters with raised evasion. If the"
+            " animation effect ID is 0,\ndefaults to animation ID 0xE (this fallback"
+            " animation likely can't be seen in normal\nplay).\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: animation effect ID\nr3: flag to"
+            " only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryActivateIdentifyCondition = Symbol(
+        [0x3B408],
+        [0x2317648],
+        None,
+        (
+            "Sets the flag for the identify orb which causes monsters holding items to"
+            " be shown with\na blue exclamation mark status icon.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictBlinkerStatus = Symbol(
+        [0x3B48C],
+        [0x23176CC],
+        None,
+        (
+            "Inflicts the Blinker status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting\nr3:"
+            " flag to log a message on failure\nreturn: Whether or not the status could"
+            " be inflicted"
+        ),
+    )
+
     IsBlinded = Symbol(
         [0x3B5A4],
         [0x23177E4],
         None,
         (
             "Returns true if the monster has the blinded status (see"
             " statuses::blinded), or if it is not the leader and is holding Y-Ray"
             " Specs.\n\nr0: pointer to entity\nr1: flag for whether to check for the"
             " held item\nreturn: bool"
         ),
     )
 
+    TryInflictCrossEyedStatus = Symbol(
+        [0x3B604],
+        [0x2317844],
+        None,
+        (
+            "Inflicts the Cross-Eyed status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEyedropStatus = Symbol(
+        [0x3B71C],
+        [0x231795C],
+        None,
+        (
+            "Inflicts the Eyedrop status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSlipStatus = Symbol(
+        [0x3B7CC],
+        [0x2317A0C],
+        None,
+        (
+            "Inflicts the Slip status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nreturn: Whether or not"
+            " the status could be inflicted"
+        ),
+    )
+
+    TryInflictDropeyeStatus = Symbol(
+        [0x3B8B4],
+        [0x2317AF4],
+        None,
+        (
+            "Inflicts the Dropeye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
     RestoreMovePP = Symbol(
         [0x3B9E0],
         [0x2317C20],
         None,
         (
             "Restores the PP of all the target's moves by the specified amount.\n\nr0:"
             " user entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3:"
             " flag to suppress message logging"
         ),
     )
 
-    SetReflectDamageCountdownTo4 = Symbol(
+    ApplyProteinEffect = Symbol(
+        [0x3BD10],
+        [0x2317F50],
+        None,
+        (
+            "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: attack boost"
+        ),
+    )
+
+    ApplyCalciumEffect = Symbol(
+        [0x3BDA4],
+        [0x2317FE4],
+        None,
+        (
+            "Tries to boost the target's special attack stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special attack boost"
+        ),
+    )
+
+    ApplyIronEffect = Symbol(
+        [0x3BE38],
+        [0x2318078],
+        None,
+        (
+            "Tries to boost the target's defense stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: defense boost"
+        ),
+    )
+
+    ApplyZincEffect = Symbol(
+        [0x3BECC],
+        [0x231810C],
+        None,
+        (
+            "Tries to boost the target's special defense stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special defense boost"
+        ),
+    )
+
+    TryInflictLongTossStatus = Symbol(
+        [0x3BF60],
+        [0x23181A0],
+        None,
+        (
+            "Inflicts the Long Toss status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictPierceStatus = Symbol(
+        [0x3BFD0],
+        [0x2318210],
+        None,
+        (
+            "Inflicts the Pierce status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictGastroAcidStatus = Symbol(
+        [0x3C03C],
+        [0x231827C],
+        None,
+        (
+            "Inflicts the Gastro Acid status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    SetAquaRingHealingCountdownTo4 = Symbol(
         [0x3C180],
         [0x23183C0],
         None,
         (
-            "Sets the monster's reflect damage countdown to a global value"
+            "Sets the countdown for Aqua Ring healing countdown to a global value"
             " (0x4).\n\nr0: pointer to entity"
         ),
     )
 
+    ApplyAquaRingHealing = Symbol(
+        [0x3C1A8],
+        [0x23183E8],
+        None,
+        (
+            "Applies the passive healing gained from the Aqua Ring status.\n\nr0:"
+            " pointer to entity"
+        ),
+    )
+
+    TryInflictAquaRingStatus = Symbol(
+        [0x3C21C],
+        [0x231845C],
+        None,
+        (
+            "Inflicts the Aqua Ring status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLuckyChantStatus = Symbol(
+        [0x3C2C8],
+        [0x2318508],
+        None,
+        (
+            "Inflicts the Lucky Chant status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictHealBlockStatus = Symbol(
+        [0x3C368],
+        [0x23185A8],
+        None,
+        (
+            "Inflicts the Heal Block status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    MonsterHasEmbargoStatus = Symbol(
+        [0x3C48C],
+        [0x23186CC],
+        None,
+        (
+            "Returns true if the monster has the Embargo status condition.\n\nr0:"
+            " pointer to entity\nreturn: bool"
+        ),
+    )
+
+    LogItemBlockedByEmbargo = Symbol(
+        [0x3C4C0],
+        [0x2318700],
+        None,
+        (
+            "Logs the error message when the usage of an item is blocked by"
+            " Embargo.\n\nr0: pointer to entity"
+        ),
+    )
+
+    TryInflictEmbargoStatus = Symbol(
+        [0x3C4EC],
+        [0x231872C],
+        None,
+        (
+            "Inflicts the Embargo status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictMiracleEyeStatus = Symbol(
+        [0x3C610],
+        [0x2318850],
+        None,
+        (
+            "Inflicts the Miracle Eye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting"
+        ),
+    )
+
+    TryInflictMagnetRiseStatus = Symbol(
+        [0x3C744],
+        [0x2318984],
+        None,
+        (
+            "Inflicts the Magnet Rise status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     HasConditionalGroundImmunity = Symbol(
         [0x3C80C],
         [0x2318A4C],
         None,
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    TryInflictSafeguardStatus = Symbol(
+        [0x3CC30],
+        [0x2318E70],
+        None,
+        (
+            "Inflicts the Safeguard status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMistStatus = Symbol(
+        [0x3CCD0],
+        [0x2318F10],
+        None,
+        (
+            "Inflicts the Mist status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWishStatus = Symbol(
+        [0x3CD6C],
+        [0x2318FAC],
+        None,
+        (
+            "Inflicts the Wish status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMagicCoatStatus = Symbol(
+        [0x3CE0C],
+        [0x231904C],
+        None,
+        (
+            "Inflicts the Magic Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLightScreenStatus = Symbol(
+        [0x3CEAC],
+        [0x23190EC],
+        None,
+        (
+            "Inflicts the Light Screen status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictReflectStatus = Symbol(
+        [0x3CF4C],
+        [0x231918C],
+        None,
+        (
+            "Inflicts the Reflect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictProtectStatus = Symbol(
+        [0x3CFEC],
+        [0x231922C],
+        None,
+        (
+            "Inflicts the Protect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorCoatStatus = Symbol(
+        [0x3D09C],
+        [0x23192DC],
+        None,
+        (
+            "Inflicts the Mirror Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictEndureStatus = Symbol(
+        [0x3D138],
+        [0x2319378],
+        None,
+        (
+            "Inflicts the Endure status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorMoveStatus = Symbol(
+        [0x3D1D8],
+        [0x2319418],
+        None,
+        (
+            "Inflicts the Mirror Move status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictConversion2Status = Symbol(
+        [0x3D278],
+        [0x23194B8],
+        None,
+        (
+            "Inflicts the Conversion2 status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictVitalThrowStatus = Symbol(
+        [0x3D344],
+        [0x2319584],
+        None,
+        (
+            "Inflicts the Vital Throw status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryResetStatChanges = Symbol(
+        [0x3D3E4],
+        [0x2319624],
+        None,
+        (
+            "Tries to reset the stat changes of the defender.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr3: bool to force animation"
+        ),
+    )
+
     MirrorMoveIsActive = Symbol(
         [0x3D508],
         [0x2319748],
         None,
         (
             "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
             " the effects is a status, 2 if it comes from an exclusive item, 0"
@@ -19346,21 +20782,101 @@
         (
             "Seems to apply an item's effect via a giant switch statement?\n\nr3:"
             " attacker pointer\nstack[0]: defender pointer\nstack[1]: thrown item"
             " pointer\nothers: ?"
         ),
     )
 
-    ViolentSeedBoost = Symbol(
+    ApplyCheriBerryEffect = Symbol(
+        [0x409AC],
+        [0x231CBEC],
+        None,
+        (
+            "Tries to heal the paralysis status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyPechaBerryEffect = Symbol(
+        [0x409D8],
+        [0x231CC18],
+        None,
+        (
+            "Tries to heal the poisoned and badly poisoned status condition. Prints a"
+            " message on\nfailure.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyRawstBerryEffect = Symbol(
+        [0x40A0C],
+        [0x231CC4C],
+        None,
+        (
+            "Tries to heal the burn status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyHungerSeedEffect = Symbol(
+        [0x40A54],
+        [0x231CC94],
+        None,
+        (
+            "Empties the targets belly to cause Hungry Pal status in non-leader"
+            " monsters and\nFamished in the leader monster.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyVileSeedEffect = Symbol(
+        [0x40B40],
+        [0x231CD80],
+        None,
+        (
+            "Reduces the targets defense and special defense stages to the lowest"
+            " level.\n\nr0: attacker pointer\nr1: defender pointer"
+        ),
+    )
+
+    ApplyViolentSeedEffect = Symbol(
         [0x40BDC],
         [0x231CE1C],
         None,
         (
-            "Applies the Violent Seed boost to an entity.\n\nr0: attacker pointer\nr1:"
-            " defender pointer"
+            "Boosts the target's offensive stats stages to the max.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGinsengEffect = Symbol(
+        [0x40C28],
+        [0x231CE68],
+        None,
+        (
+            "Boosts the power of the move at the top of the target's Move List. Appears"
+            " to have a\nleftover check to boost the power of a move by 3 instead of 1"
+            " that always fails because\nthe chance is 0.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyBlastSeedEffect = Symbol(
+        [0x40D44],
+        [0x231CF84],
+        None,
+        (
+            "If thrown, unfreeze and deal fixed damage to the defender. If not thrown,"
+            " try to find \na monster in front of the attacker. If a monster is found"
+            " unfreeze and dedal fixed \ndamage to the defender. Appears to have a"
+            " leftover check for if the current fixed room is a boss fight and loads a"
+            " different pointer for the damage when used in a boss room.\nHowever, this"
+            " isn't noticeable because both the normal and boss damage is the"
+            " same.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: bool"
+            " thrown"
         ),
     )
 
     ApplyGummiBoostsDungeonMode = Symbol(
         [0x40E80],
         [0x231D0C0],
         None,
@@ -19402,14 +20918,68 @@
         None,
         (
             "If the target monster is a Linoone, restores all the PP of all the"
             " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
+    ApplyDoughSeedEffect = Symbol(
+        [0x414A0],
+        [0x231D6E0],
+        None,
+        (
+            "If the target monster is a team member, set dough_seed_extra_poke_flag to"
+            " true to \nmake extra poke spawn on the next floor. Otherwise, do"
+            " nothing.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyViaSeedEffect = Symbol(
+        [0x4150C],
+        [0x231D74C],
+        None,
+        (
+            "Tries to randomly teleport the target with a message for eating the"
+            " seed.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGravelyrockEffect = Symbol(
+        [0x41580],
+        [0x231D7C0],
+        None,
+        (
+            "Restores 10 hunger to the target and will raise the target's IQ if they"
+            " are a bonsly\nor sudowoodo.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyGonePebbleEffect = Symbol(
+        [0x415F8],
+        [0x231D838],
+        None,
+        (
+            "Causes a few visual effects, temporarily changes the dungeon music to the"
+            " Goodnight\ntrack, and gives the target the enduring status.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGracideaEffect = Symbol(
+        [0x41780],
+        [0x231D9C0],
+        None,
+        (
+            "If the target is Shaymin, attempt to change the target's form to Shaymin"
+            " Sky Forme. Otherwise, do nothing.\n\nr0: user entity pointer\nr1: target"
+            " entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         [0x42750],
         [0x231E990],
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -19476,22 +21046,36 @@
         (
             "Blows away the target monster in a given direction if possible.\n\nr0:"
             " user entity pointer\nr1: target entity pointer\nr2: direction ID"
         ),
     )
 
     TryExplosion = Symbol(
-        [0x44548],
-        [0x2320788],
+        [0x44208],
+        [0x2320448],
         None,
         (
             "Creates an explosion if possible.\n\nThe target monster is considered the"
             " source of the explosion.\n\nr0: user entity pointer\nr1: target entity"
             " pointer\nr2: coordinates where the explosion should take place"
-            " (unverified)\nr3: ?\nstack[0]: ?\nstack[1]: damage source (normally"
+            " (center)\nr3: explosion radius (only works correctly with 1 and"
+            " 2)\nstack[0]: damage type\nstack[1]: damage source"
+        ),
+    )
+
+    TryAftermathExplosion = Symbol(
+        [0x44548],
+        [0x2320788],
+        None,
+        (
+            "Creates the explosion for the ability aftermath if possible.\n\nThe target"
+            " monster is considered the source of the explosion.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: coordinates where the explosion"
+            " should take place (center)\nr3: explosion radius (only works correctly"
+            " with 1 and 2)\nstack[0]: damage type\nstack[1]: damage source (normally"
             " DAMAGE_SOURCE_EXPLOSION)"
         ),
     )
 
     TryWarp = Symbol(
         [0x44AC8],
         [0x2320D08],
@@ -19965,14 +21549,57 @@
     GetStairsRoom = Symbol(
         [0x5A1E8],
         [0x2336428],
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    UpdateTrapsVisibility = Symbol(
+        [0x5AD0C],
+        [0x2336F4C],
+        None,
+        (
+            "Exact purpose unknown. Gets called whenever a trap tile is shown or"
+            " hidden.\n\nNo params."
+        ),
+    )
+
+    DrawTileGrid = Symbol(
+        [0x5B1E8],
+        [0x2337428],
+        None,
+        (
+            "Draws a grid on the nearby walkable tiles. Triggered by pressing Y.\n\nr0:"
+            " Coordinates of the entity around which the grid will be drawn\nr1: ?\nr2:"
+            " ?\nr3: ?"
+        ),
+    )
+
+    HideTileGrid = Symbol(
+        [0x5B55C],
+        [0x233779C],
+        None,
+        (
+            "Hides the grid on the nearby walkable tiles. Triggered by releasing"
+            " Y.\n\nNo params."
+        ),
+    )
+
+    DiscoverMinimap = Symbol(
+        [0x5B7FC],
+        [0x2337A3C],
+        None,
+        (
+            "Discovers the tiles around the specified position on the minimap.\n\nThe"
+            " discovery radius depends on the visibility range of the floor. If"
+            " display_data::blinded is true, the function returns early without doing"
+            " anything.\n\nr0: Position around which the map should be discovered"
+        ),
+    )
+
     IsWaterTileset = Symbol(
         [0x5BC54],
         [0x2337E94],
         None,
         (
             "Returns flag tileset_property::is_water_tileset for the current"
             " tileset\n\nreturn: True if the current tileset is a water tileset"
@@ -20041,14 +21668,34 @@
         (
             "Sets the boost_kecleon_shop_spawn_chance field on the dungeon struct"
             " depending on if a team member has the exclusive item effect for more"
             " kecleon shops.\n\nNo params."
         ),
     )
 
+    SetDoughSeedFlag = Symbol(
+        [0x5C308],
+        [0x2338548],
+        None,
+        (
+            "Sets the dough_seed_extra_money_flag field on the dungeon struct to the"
+            " given value.\n\nr0: bool to set the flag to"
+        ),
+    )
+
+    TrySpawnDoughSeedPoke = Symbol(
+        [0x5C320],
+        [0x2338560],
+        None,
+        (
+            "Checks the dough_seed_extra_money_flag field on the dungeon struct and"
+            " tries to spawn\nextra poke if it is set.\n\nNo params."
+        ),
+    )
+
     IsSecretBazaar = Symbol(
         [0x5C384],
         [0x23385C4],
         None,
         "Checks if the current floor is the Secret Bazaar.\n\nreturn: bool",
     )
 
@@ -20099,28 +21746,62 @@
         None,
         (
             "Checks if the current floor is a secret bazaar or a secret"
             " room.\n\nreturn: bool"
         ),
     )
 
+    HiddenStairsPresent = Symbol(
+        [0x5C498],
+        [0x23386D8],
+        None,
+        (
+            "Checks if the hidden stairs are present on this floor.\n\nThe function"
+            " checks that dungeon_generation_info::hidden_stairs_pos isn't (-1,"
+            " -1)\n\nreturn: True if the hidden stairs are present on this floor, false"
+            " otherwise."
+        ),
+    )
+
+    HiddenStairsTrigger = Symbol(
+        [0x5C554],
+        [0x2338794],
+        None,
+        (
+            "Called whenever the leader steps on the hidden stairs.\n\nIf the stairs"
+            " hadn't been revealed yet, plays the corresponding animation.\n\nr0: True"
+            " to display a message if the stairs are revealed, false to omit it."
+        ),
+    )
+
     GetDungeonGenInfoUnk0C = Symbol(
         [0x5C640], [0x2338880], None, "return: dungeon_generation_info::field_0xc"
     )
 
     GetMinimapData = Symbol(
         [0x5CED8],
         [0x2339118],
         None,
         (
             "Returns a pointer to the minimap_display_data struct in the dungeon"
             " struct.\n\nreturn: minimap_display_data*"
         ),
     )
 
+    DrawMinimapTile = Symbol(
+        [0x5CFAC],
+        [0x23391EC],
+        None,
+        "Draws a single tile on the minimap.\n\nr0: X position\nr1: Y position",
+    )
+
+    UpdateMinimap = Symbol(
+        [0x5DAA8], [0x2339CE8], None, "Graphically updates the minimap\n\nNo params."
+    )
+
     SetMinimapDataE447 = Symbol(
         [0x5DFD8],
         [0x233A218],
         None,
         (
             "Sets minimap_display_data::field_0xE447 to the specified value\n\nr0:"
             " Value to set the field to"
@@ -20144,14 +21825,35 @@
         None,
         (
             "Sets minimap_display_data::field_0xE448 to the specified value\n\nr0:"
             " Value to set the field to"
         ),
     )
 
+    InitWeirdMinimapMatrix = Symbol(
+        [0x5E050],
+        [0x233A290],
+        None,
+        (
+            "Initializes the matrix at minimap_display_data+0xE000. Seems to overflow"
+            " said matrix when doing so.\n\nNo params."
+        ),
+    )
+
+    InitMinimapDisplayTile = Symbol(
+        [0x5E0B0],
+        [0x233A2F0],
+        None,
+        (
+            "Used to initialize an instance of struct minimap_display_tile\n\nr0:"
+            " Pointer to struct to init\nr1: Seems to be a pointer to the file that"
+            " stores minimap icons or something like that"
+        ),
+    )
+
     LoadFixedRoomDataVeneer = Symbol(
         [0x5E3E4],
         [0x233A624],
         None,
         (
             "Likely a linker-generated veneer for LoadFixedRoomData.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nNo"
@@ -20843,14 +22545,24 @@
             " reached by the traversal algorithm, then the stairs must not be reachable"
             " from that tile.\n\nr0: x coordinate of the stairs\nr1: y coordinate of"
             " the stairs\nr2: flag to always return true, but set a special bit on all"
             " walkable tiles that aren't reachable from the stairs\nreturn: bool"
         ),
     )
 
+    GetNextFixedRoomAction = Symbol(
+        [0x66290],
+        [0x23424D0],
+        None,
+        (
+            "Returns the next action that needs to be performed when spawning a fixed"
+            " room tile.\n\nreturn: Next action ID"
+        ),
+    )
+
     ConvertWallsToChasms = Symbol(
         [0x66308], [0x2342548], None, "Converts all wall tiles to chasms.\n\nNo params."
     )
 
     ResetInnerBoundaryTileRows = Symbol(
         [0x6693C],
         [0x2342B7C],
@@ -20901,25 +22613,75 @@
             " HIDDEN_STAIRS_RANDOM_SECRET_BAZAAR_OR_SECRET_ROOM and the"
             " floor_properties::hidden_stairs_spawn_chance) into a concrete hidden"
             " stairs type.\n\nr0: dungeon generation info pointer\nr1: floor properties"
             " pointer\nreturn: enum hidden_stairs_type"
         ),
     )
 
+    GetFinalKecleonShopSpawnChance = Symbol(
+        [0x66C7C],
+        [0x2342EBC],
+        None,
+        (
+            "Gets the kecleon shop spawn chance for the floor.\n\nWhen"
+            " dungeon::boost_kecleon_shop_spawn_chance is false, returns the same value"
+            " as the input. When it's true, returns the input (chance * 1.2).\n\nr0:"
+            " base kecleon shop spawn chance,"
+            " floor_properties::kecleon_shop_spawn_chance\nreturn: int"
+        ),
+    )
+
     ResetHiddenStairsSpawn = Symbol(
         [0x66CC8],
         [0x2342F08],
         None,
         (
             "Resets hidden stairs spawn information for the floor. This includes the"
             " position on the floor generation status as well as the flag indicating"
             " whether the spawn was blocked.\n\nNo params."
         ),
     )
 
+    PlaceFixedRoomTile = Symbol(
+        [0x66CF0],
+        [0x2342F30],
+        None,
+        (
+            "Used to spawn a single tile when generating a fixed room. The tile might"
+            " contain an item or a monster.\n\nr0: Pointer to the tile to spawn\nr1:"
+            " Fixed room action to perform. Controls what exactly will be spawned. The"
+            " action is actually 12 bits long, the highest 4 bits are used as a"
+            " parameter that represents a direction (for example, when spawning a"
+            " monster).\nr2: Tile X position\nr3: Tile Y position"
+        ),
+    )
+
+    FixedRoomActionParamToDirection = Symbol(
+        [0x6772C],
+        [0x234396C],
+        None,
+        (
+            "Converts the parameter stored in a fixed room action value to a direction"
+            " ID.\n\nThe conversion is performed by subtracting 1 to the value. If the"
+            " parameter had a value of 0, DIR_NONE is returned.\n\nr0: Parameter"
+            " value\nreturn: Direction"
+        ),
+    )
+
+    ApplyKeyEffect = Symbol(
+        [0x67A98],
+        [0x2343CD8],
+        None,
+        (
+            "Attempts to open a locked door in front of the target if a locked door has"
+            " not already\nbeen open on the floor.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
     LoadFixedRoomData = Symbol(
         [0x67B50],
         [0x2343D90],
         None,
         (
             "Loads fixed room data from BALANCE/fixed.bin into the buffer pointed to by"
             " FIXED_ROOM_DATA_PTR.\n\nNo params."
@@ -21702,15 +23464,25 @@
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
             " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
     OpenMenu = Symbol(
-        [0x71BB4], [0x234DDF4], None, "Note: unverified, ported from Irdkwia's notes"
+        [0x71BB4],
+        [0x234DDF4],
+        None,
+        (
+            "Opens a menu. The menu to open depends on the specified parameter.\n\nIt"
+            " looks like the function takes a parameter in r0, but doesn't use it. r1"
+            " doesn't even get set when this function is called.\n\nr0: (?) Unused by"
+            " the function. Seems to be 1 byte long.\nr1: (?) Unused by the function."
+            " Seems to be 1 byte long.\nr2: True to open the bag menu, false to open"
+            " the main dungeon menu"
+        ),
     )
 
     OthersMenuLoop = Symbol(
         [0x73580],
         [0x234F7C0],
         None,
         (
@@ -21904,27 +23676,30 @@
         0x4,
         (
             "The move target and range code for special healing moves that target just"
             " the user (0x273).\n\ntype: struct move_target_and_range (+ padding)"
         ),
     )
 
-    PLAIN_SEED_VALUE = Symbol(
-        [0x40508], [0x231C748], 0x4, "Some value related to the Plain Seed (0xBE9)."
+    PLAIN_SEED_STRING_ID = Symbol(
+        [0x40508], [0x231C748], 0x4, "The string ID for eating a Plain Seed (0xBE9)."
     )
 
     MAX_ELIXIR_PP_RESTORATION = Symbol(
         [0x4050C],
         [0x231C74C],
         0x4,
         "The amount of PP restored per move by ingesting a Max Elixir (0x3E7).",
     )
 
-    SLIP_SEED_VALUE = Symbol(
-        [0x4096C], [0x231CBAC], 0x4, "Some value related to the Slip Seed (0xC75)."
+    SLIP_SEED_FAIL_STRING_ID = Symbol(
+        [0x4096C],
+        [0x231CBAC],
+        0x4,
+        "The string ID for when eating the Slip Seed fails (0xC75).",
     )
 
     ROCK_WRECKER_MOVE_ID = Symbol(
         [0x48360], [0x23245A0], 0x4, "The move ID for Rock Wrecker (453)."
     )
 
     CASTFORM_NORMAL_FORM_MALE_ID = Symbol(
@@ -22769,15 +24544,28 @@
     loadaddress = 0x233CA80
     length = 0xA160
     functions = NaOverlay3Functions
     data = NaOverlay3Data
 
 
 class NaOverlay30Functions:
-    pass
+    WriteQuicksaveData = Symbol(
+        [0x44C],
+        [0x2382C6C],
+        None,
+        (
+            "Function responsible for writing dungeon data when quicksaving.\n\nAmong"
+            " other things, it contains a loop that goes through all the monsters in"
+            " the current dungeon, copying their data to the buffer. The data is not"
+            " copied as-is though, the game uses a reduced version of the monster"
+            " struct containing only the minimum required data to resume the game"
+            " later.\n\nr0: Pointer to buffer where data should be written\nr1: Buffer"
+            " size. Seems to be 0x5800 (22 KB) when the function is called."
+        ),
+    )
 
 
 class NaOverlay30Data:
     OVERLAY30_JP_STRING_1 = Symbol([0x3860], [0x2386080], 0xC, "みさき様")
 
     OVERLAY30_JP_STRING_2 = Symbol([0x386C], [0x238608C], 0xC, "やよい様")
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -1020,17 +1020,17 @@
 
     LoadFileInPackWithPackId = Symbol(
         None,
         None,
         None,
         (
             "Call LoadFileInPack after looking up the global Pack archive by its"
-            " identifier\n\nr0: pack file identifier\nr1: [output] target buffer\nr2:"
-            " file index\nreturn: number of read bytes (identical to the length of the"
-            " pack from the Table of Content)"
+            " identifier\n\nr0: pack file identifier\nr1: file index\nr2: [output]"
+            " target buffer\nreturn: number of read bytes (identical to the length of"
+            " the pack from the Table of Content)"
         ),
     )
 
     AllocAndLoadFileInPack = Symbol(
         None,
         None,
         None,
@@ -1071,14 +1071,27 @@
             "Load the indexed file from the Pack archive, itself loaded from the"
             " ROM.\n\nr0: pack file struct\nr1: [output] target buffer\nr2: file"
             " index\nreturn: number of read bytes (identical to the length of the pack"
             " from the Table of Content)"
         ),
     )
 
+    GetDungeonResultMsg = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the message that is shown on the dungeon results ('The Last Outing')"
+            " screen, right after the leader's name.\n\nr0: Damage source value to use"
+            " when displaying the cause of fainting or the result of the"
+            " expedition\nr1: [output] Buffer where the resulting message will be"
+            " stored\nr2: Buffer size\nr3: (?) Seems to point to a buffer"
+        ),
+    )
+
     GetDamageSource = Symbol(
         None,
         None,
         None,
         (
             "Gets the damage source for a given move-item combination.\n\nIf there's no"
             " item, the source is the move ID. If the item is an orb, return"
@@ -1153,14 +1166,26 @@
         None,
         (
             "Checks if an item is one of the aura bows received at the start of the"
             " game.\n\nr0: item ID\nreturn: bool"
         ),
     )
 
+    IsTreasureBox = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the given item ID is a treasure box\n\nIn particular, it checks"
+            " if the category of the item is CATEGORY_TREASURE_BOXES_1,"
+            " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
+            " ID\nreturn: True if the item is a treasure box, false otherwise"
+        ),
+    )
+
     InitItem = Symbol(
         None,
         None,
         None,
         (
             "Initialize an item struct with the given information.\n\nThis will resolve"
             " the quantity based on the item type. For Poké, the quantity code will"
@@ -1441,22 +1466,21 @@
     GetItemMoveId = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: move ID",
     )
 
-    TestItemFlag0xE = Symbol(
+    TestItemAiFlag = Symbol(
         None,
         None,
         None,
         (
-            "Tests bit 7 if r1 is 0, bit 6 if r1 is 1, bit 5 otherwise\n\nNote:"
-            " unverified, ported from Irdkwia's notes\n\nr0: item ID\nr1:"
-            " bit_id\nreturn: bool"
+            "Used to check the AI flags for an item. Tests bit 7 if r1 is 0, bit 6 if"
+            " r1 is 1, bit\n5 otherwise.\n\nr0: item ID\nr1: bit_id\nreturn: bool"
         ),
     )
 
     IsItemInTimeDarkness = Symbol(
         None,
         None,
         None,
@@ -1494,14 +1518,25 @@
         None,
         (
             "Sets the amount of money the player is carrying, clamping the value to the"
             " range [0, MAX_MONEY_CARRIED].\n\nr0: new value"
         ),
     )
 
+    AddMoneyCarried = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds the amount of money to the player's current amount of money. Just"
+            " calls\nSetMoneyCarried with the current money + money gained.\n\nr0:"
+            " money gained (can be negative)"
+        ),
+    )
+
     GetCurrentBagCapacity = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: bag capacity",
     )
 
@@ -1522,15 +1557,18 @@
         "Note: unverified, ported from Irdkwia's notes\n\nreturn: # items",
     )
 
     CountNbItemsOfTypeInBag = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: item ID\nreturn: count",
+        (
+            "Returns the number of items of the given kind in the bag\n\nr0: item"
+            " ID\nreturn: count"
+        ),
     )
 
     CountItemTypeInBag = Symbol(
         None,
         None,
         None,
         (
@@ -1742,14 +1780,24 @@
     ScriptSpecialProcess0x39 = Symbol(
         None,
         None,
         None,
         "Implements SPECIAL_PROC_0x39 (see ScriptSpecialProcessCall).\n\nreturn: bool",
     )
 
+    CountNbItemsOfTypeInStorage = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the number of items of the given kind in the storage\n\nr0: item"
+            " ID\nreturn: count"
+        ),
+    )
+
     CountItemTypeInStorage = Symbol(
         None,
         None,
         None,
         (
             "Implements SPECIAL_PROC_COUNT_ITEM_TYPE_IN_STORAGE (see"
             " ScriptSpecialProcessCall).\n\nr0: pointer to an owned_item\nreturn:"
@@ -2588,38 +2636,62 @@
     StopSe = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
 
     DeleteWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
+            "Always delete an entry if the file is allocated externally"
+            " (file_externally_allocated is set), otherwise, decrease the reference"
+            " counter. If it reach 0, delete the sprite.\n\nr0: wan_table_ptr\nr1:"
             " wan_id"
         ),
     )
 
+    AllocateWanTableEntry = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return the identifier to a free wan table entry (-1 if none are"
+            " avalaible). The entry is zeroed.\n\nr0: wan_table_ptr\nreturn: the entry"
+            " id in wan_table"
+        ),
+    )
+
     FindWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Appears to search in the given table (in practice always seems to be"
+            "Search in the given table (in practice always seems to be"
             " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
             " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
             " if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "wan_id = -1 if it is not loaded\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: wan_table_ptr\nr1: bin_file_id\nr2: file_id\nreturn: wan_id"
+            "Look up a sprite with the provided pack_id and file_index in the wan"
+            " table.\n\nr0: wan_table_ptr\nr1: pack_id\nr2: file_index\nreturn: sprite"
+            " id in the wan table, -1 if not found"
+        ),
+    )
+
+    InitWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the input WAN table with 0x60 free entries (it needs a length"
+            " of 0x1510 bytes)\n\nr0: wan_table_ptr"
         ),
     )
 
     LoadWanTableEntry = Symbol(
         None,
         None,
         None,
@@ -2627,14 +2699,40 @@
             "Appears to load data from the given file (in practice always seems to be"
             " animation data), using previously loaded data in the given table (see"
             " FindWanTableEntry) if possible.\n\nr0: table pointer\nr1: file name\nr2:"
             " flags\nreturn: table index of the loaded data"
         ),
     )
 
+    LoadWanTableEntryFromPack = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3: allocation"
+            " flags\nstack[0]: compressed\nreturn: the entry id in wan_table"
+        ),
+    )
+
+    LoadWanTableEntryFromPackUseProvidedMemory = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Return an already allocated entry for this sprite if it exists, otherwise"
+            " allocate a new one and load the optionally compressed sprite into the"
+            " provided memory area. Mark the sprite as externally allocated.\n\nr0:"
+            " wan_table_ptr\nr1: pack_id\nr2: file_index\nr3:"
+            " sprite_storage_ptr\nstack[0]: compressed\nreturn: the entry id in"
+            " wan_table"
+        ),
+    )
+
     ReplaceWanFromBinFile = Symbol(
         None,
         None,
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: wan_table_ptr\nr1:"
             " wan_id\nr2: bin_file_id\nr3: file_id\nstack[0]: compressed"
@@ -2890,14 +2988,30 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetStringPower = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
+    GetDungeonResultString = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns a string containing some information to be used when displaying"
+            " the dungeon results screen.\n\nThe exact string returned depends on the"
+            " value of r0:\n0: Name of the move that fainted the leader. Empty string"
+            " if the leader didn't faint.\n1-3: Seems to always result in an empty"
+            " string.\n4: Name of the pokémon that fainted the leader, or name of the"
+            " leader if the leader didn't faint.\n5: Name of the fainted leader. Empty"
+            " string if the leader didn't faint.\n\nr0: String to return\nreturn:"
+            " Pointer to resulting string"
+        ),
+    )
+
     SetQuestionMarks = Symbol(
         None,
         None,
         None,
         (
             "Fills the buffer with the string '???'\n\nNote: unverified, ported from"
             " Irdkwia's notes\n\nr0: buffer"
@@ -3196,15 +3310,15 @@
 
     IsMenuOptionActive = Symbol(
         None,
         None,
         None,
         (
             "Called whenever a menu option is selected. Returns whether the option is"
-            " active or not.\n\nr0: ?\nReturn: True if the menu option is enabled,"
+            " active or not.\n\nr0: ?\nreturn: True if the menu option is enabled,"
             " false otherwise."
         ),
     )
 
     ShowKeyboard = Symbol(
         None,
         None,
@@ -3570,14 +3684,24 @@
         None,
         (
             "Gets the special episode type from the SPECIAL_EPISODE_TYPE script"
             " variable.\n\nreturn: special episode type"
         ),
     )
 
+    GetExecuteSpecialEpisodeType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the special episode type from the EXECUTE_SPECIAL_EPISODE_TYPE script"
+            " variable.\n\nreturn: special episode type"
+        ),
+    )
+
     HasPlayedOldGame = Symbol(
         None,
         None,
         None,
         "Returns the value of the VAR_PLAY_OLD_GAME script variable.\n\nreturn: bool",
     )
 
@@ -3640,21 +3764,21 @@
         None,
         (
             "Note: unverified, ported from Irdkwia's notes\n\nr0: dungeon ID\nr1:"
             " bit_value"
         ),
     )
 
-    CheckDungeonOpen = Symbol(
+    GetDungeonMode = Symbol(
         None,
         None,
         None,
         (
-            "Related to dungeon open list\n\nNote: unverified, ported from Irdkwia's"
-            " notes\n\nr0: dungeon ID\nreturn: status code?"
+            "Returns the mode of the specified dungeon\n\nr0: Dungeon ID\nreturn:"
+            " Dungeon mode"
         ),
     )
 
     GlobalProgressAlloc = Symbol(
         None,
         None,
         None,
@@ -3861,14 +3985,59 @@
         (
             "If buffer_portrait is null, it only checks if it exists\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: portrait box pointer\nr1:"
             " buffer_portrait\nreturn: exists"
         ),
     )
 
+    SetEnterDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to set the dungeon that will be accessed when switching from ground"
+            " to dungeon mode.\n\nr0: Dungeon ID"
+        ),
+    )
+
+    InitDungeonInit = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the dungeon_init struct before entering a dungeon.\n\nr0:"
+            " [output] Pointer to the struct to init\nr1: Dungeon ID"
+        ),
+    )
+
+    IsNoLossPenaltyDungeon = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the specified dungeon shouldn't have a loss penalty.\n\nIf"
+            " true you won't lose your money and items upon fainting. Also used to"
+            " initialize dungeon_init::skip_faint_animation_flag.\n\nReturns: True for"
+            " DUNGEON_CRYSTAL_LAKE and DUNGEON_5TH_STATION_CLEARING, as well as for"
+            " DUNGEON_DEEP_STAR_CAVE_TEAM_ROGUE if the ground variable SIDE01_BOSS2ND"
+            " is 0; false otherwise."
+        ),
+    )
+
+    CheckMissionRestrictions = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Seems to be used to check if you have any missions that have unmet"
+            " restrictions when trying to access a dungeon.\n\nr0: ?\nreturn: (?) Seems"
+            " to be composed of multiple bitflags."
+        ),
+    )
+
     GetNbFloors = Symbol(
         None,
         None,
         None,
         (
             "Returns the number of floors of the given dungeon.\n\nThe result is"
             " hardcoded for certain dungeons, such as dojo mazes.\n\nr0: Dungeon"
@@ -3930,19 +4099,75 @@
         (
             "Given a dungeon ID and a floor number, returns a struct with the"
             " corresponding dungeon group and floor number in that group.\n\nThe"
             " function normally uses the data in mappa_s.bin to calculate the result,"
             " but there's some dungeons (such as dojo mazes) that have hardcoded return"
             " values.\n\nIrdkwia's notes:\n  [r1]: dungeon_id\n  [r1+1]:"
             " dungeon_floor_id\n  [r0]: group_id\n  [r0+1]: group_floor_id\n\nr0:"
-            " (output) Struct containing the dungeon group and floor group\nr1: Struct"
+            " [output] Struct containing the dungeon group and floor group\nr1: Struct"
             " containing the dungeon ID and floor number"
         ),
     )
 
+    GetMissionRank = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the mission rank for the given dungeon and floor.\n\nIf the dungeon"
+            " ID is >= DUNGEON_NORMAL_FLY_MAZE or the group of the dungeon is >"
+            " DGROUP_DUMMY_0x63, returns MISSION_RANK_E.\n\nr0: Dungeon and"
+            " floor\nreturn: Mission rank"
+        ),
+    )
+
+    GetOutlawLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for outlaws for the given dungeon and"
+            " floor\n\nr0: Dungeon and floor\nreturn: Outlaw level"
+        ),
+    )
+
+    GetOutlawLeaderLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for team leader outlaws for the given"
+            " dungeon and floor. Identical to GetOutlawLevel.\n\nr0: Dungeon and"
+            " floor\nreturn: Outlaw leader level"
+        ),
+    )
+
+    GetOutlawMinionLevel = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the level that should be used for minion outlaws for the given"
+            " dungeon and floor.\n\nr0: Dungeon and floor\nreturn: Outlaw minion level"
+        ),
+    )
+
+    AddGuestMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Adds a guest monster to the active team\n\nr0: dungeon_init struct for the"
+            " dungeon that is about to be entered\nr1: Number of the guest monster to"
+            " add. Used when more than one monster is added.\nr2: Pointer to the guest"
+            " monster entry to add to the team (usually located within"
+            " GUEST_MONSTER_DATA)"
+        ),
+    )
+
     GetGroundNameId = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     SetAdventureLogStructLocation = Symbol(
         None,
         None,
@@ -5010,14 +5235,24 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: family index",
     )
 
     LoadM2nAndN2m = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    GuestMonsterToGroundMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inits a ground_monster entry with the given guest_monster struct.\n\nr0:"
+            " [output] ground_monster struct to init\nr1: guest_monster struct to use"
+        ),
+    )
+
     StrcmpMonsterName = Symbol(
         None,
         None,
         None,
         (
             "Checks if the string_buffer matches the name of the species\n\nNote:"
             " unverified, ported from Irdkwia's notes\n\nr0: string_buffer\nr1: monster"
@@ -5586,15 +5821,15 @@
         None,
         None,
         None,
         (
             "Determines the list of IQ skills that a given monster can learn given its"
             " IQ value.\n\nThe list of skills is written in the array specified in r0."
             " The array has 69 slots in total. Unused slots are set to 0.\n\nr0:"
-            " (output) Array where the list of skills will be written\nr1: Monster"
+            " [output] Array where the list of skills will be written\nr1: Monster"
             " species\nr2: Monster IQ\nreturn: Amount of skills written to the output"
             " array"
         ),
     )
 
     DisableIqSkill = Symbol(
         None,
@@ -6023,26 +6258,121 @@
         (
             "Converts an index in DUNGEON_SWAP_ID_TABLE to the corresponding dungeon"
             " ID, or DUNGEON_DUMMY_0xFF if the index is -1.\n\nr0: index\nreturn:"
             " dungeon ID"
         ),
     )
 
+    GetDungeonModeSpecial = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the status of the given dungeon, with some modifications.\n\nIf"
+            " the dungeon ID is DUNGEON_BEACH, returns DMODE_REQUEST.\nIf it's"
+            " DUNGEON_JOINED_AT_UNKNOWN, returns DMODE_OPEN_AND_REQUEST.\nIf it's >="
+            " DUNGEON_NORMAL_FLY_MAZE and <= DUNGEON_DOJO_0xD3, returns"
+            " DMODE_OPEN_AND_REQUEST.\nElse, calls GetDungeonMode and returns"
+            " DMODE_REQUEST if the dungeon has been cleared, or DMODE_OPEN if it's"
+            " not.\n\nr0: Dungeon ID\nreturn: Dungeon mode"
+        ),
+    )
+
     ResumeBgm = Symbol(
         None, None, None, "Uncertain.\n\nNote: unverified, ported from Irdkwia's notes"
     )
 
     FlushChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes"
     )
 
     UpdateChannels = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nNo params."
     )
 
+    ClearIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Enables processor interrupts by clearing the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were disabled, 0x0 if they were already enabled)"
+        ),
+    )
+
+    EnableIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Disables processor interrupts by setting the i flag in the program status"
+            " register (cpsr).\n\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts"
+            " were already disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    SetIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the value of the processor's interrupt flag according to the"
+            " specified parameter.\n\nr0: Value to set the flag to (0x80 to set it,"
+            " which disables interrupts; 0x0 to unset it, which enables"
+            " interrupts)\nreturn: Old value of cpsr & 0x80 (0x80 if interrupts were"
+            " disabled, 0x0 if they were enabled)"
+        ),
+    )
+
+    EnableIrqFiqFlags = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Disables processor all interrupts (both standard and fast) by setting the"
+            " i and f flags in the program status register (cpsr).\n\nreturn: Old value"
+            " of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    SetIrqFiqFlags = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the value of the processor's interrupt flags (i and f) according to"
+            " the specified parameter.\n\nr0: Value to set the flags to (0xC0 to set"
+            " both flags, 0x80 to set the i flag and clear the f flag, 0x40 to set the"
+            " f flag and clear the i flag and 0x0 to clear both flags)\nreturn: Old"
+            " value of cpsr & 0xC0 (contains the previous values of the i and f flags)"
+        ),
+    )
+
+    GetIrqFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the current value of the processor's interrupt request (i)"
+            " flag\n\nreturn: cpsr & 0x80 (0x80 if interrupts are disabled, 0x0 if they"
+            " are enabled)"
+        ),
+    )
+
+    WaitForever2 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EnableIrqFlag and WaitForInterrupt in an infinite loop.\n\nThis is"
+            " called on fatal errors to hang the program indefinitely.\n\nNo params."
+        ),
+    )
+
     WaitForInterrupt = Symbol(
         None,
         None,
         None,
         (
             "Presumably blocks until the program receives an interrupt.\n\nThis just"
             " calls (in Ghidra terminology) coproc_moveto_Wait_for_interrupt(0). See"
@@ -12617,14 +12947,24 @@
         None,
         (
             "The multiplier for damage from the Air Blade (1.5), as a binary"
             " fixed-point number (8 fraction bits)"
         ),
     )
 
+    KECLEON_SHOP_BOOST_CHANCE_MULTIPLIER = Symbol(
+        None,
+        None,
+        None,
+        (
+            "The boosted kecleon shop spawn chance multiplier (~1.2) as a binary"
+            " fixed-point number (8 fraction bits)."
+        ),
+    )
+
     HIDDEN_STAIRS_SPAWN_CHANCE_MULTIPLIER = Symbol(
         None,
         None,
         None,
         (
             "The hidden stairs spawn chance multiplier (~1.2) as a binary fixed-point"
             " number (8 fraction bits), if applicable. See"
@@ -13301,16 +13641,18 @@
     )
 
     LoadBackgroundAttributes = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: [output]"
-            " bg_attr_str\nr1: bg_id"
+            "Open and read an entry from the MAP_BG/bg_list.dat\n\nDocumentation on"
+            " this format can be found"
+            " here:\nhttps://github.com/SkyTemple/skytemple-files/tree/55b3017631a8a1b0f106111ef91a901dc394c6df/skytemple_files/graphics/bg_list_dat\n\nr0:"
+            " [output] The entry\nr1: background ID"
         ),
     )
 
     LoadMapType10 = Symbol(
         None,
         None,
         None,
@@ -13413,14 +13755,24 @@
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
             " characters printed, excluding the null-terminator"
         ),
     )
 
+    GetExclusiveItemRequirements = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to calculate the items required to get a certain exclusive item in"
+            " the swap shop.\n\nr0: ?\nr1: ?"
+        ),
+    )
+
     StatusUpdate = Symbol(
         None,
         None,
         None,
         (
             "Implements SPECIAL_PROC_STATUS_UPDATE (see"
             " ScriptSpecialProcessCall).\n\nNo params."
@@ -13579,14 +13931,18 @@
         ),
     )
 
     UNIONALL_RAM_ADDRESS = Symbol(None, None, None, "[Runtime]")
 
     GROUND_STATE_MAP = Symbol(None, None, None, "[Runtime]")
 
+    GROUND_STATE_WEATHER = Symbol(
+        None, None, None, "[Runtime] Same structure format as GROUND_STATE_MAP"
+    )
+
     GROUND_STATE_PTRS = Symbol(
         None,
         None,
         None,
         (
             "Host pointers to multiple structure used for performing an overworld"
             " scene\n\ntype: struct main_ground_data"
@@ -15430,24 +15786,81 @@
     FadeToBlack = Symbol(
         None,
         None,
         None,
         "Fades the screen to black across several frames.\n\nNo params.",
     )
 
+    CheckTouchscreenArea = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the currently pressed touchscreen position is within the"
+            " specified area.\n\nr0: Area lower X coordinate\nr1: Area lower Y"
+            " coordinate\nr2: Area upper X coordinate\nr3: Area upper Y"
+            " coordinate\nreturn: True if the specified area contains the currently"
+            " pressed touchscreen position, false otherwise."
+        ),
+    )
+
+    GetTrapInfo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Given a trap entity, returns the pointer to the trap info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Trap data pointer"
+        ),
+    )
+
+    GetItemInfo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Given an item entity, returns the pointer to the item info struct it"
+            " contains.\n\nr0: Entity pointer\nreturn: Item data pointer"
+        ),
+    )
+
     GetTileAtEntity = Symbol(
         None,
         None,
         None,
         (
             "Returns a pointer to the tile where an entity is located.\n\nr0: pointer"
             " to entity\nreturns: pointer to tile"
         ),
     )
 
+    UpdateEntityPixelPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Updates an entity's pixel_pos field using the specified pixel_position"
+            " struct, or its own pos field if it's null.\n\nr0: Entity pointer\nr1:"
+            " Pixel position to use, or null to use the entity's own position"
+        ),
+    )
+
+    CreateEnemyEntity = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Creates and initializes the entity struct of a newly spawned enemy"
+            " monster. Fails if there's 16 enemies on the floor already.\n\nIt could"
+            " also be used to spawn fixed room allies, since those share their slots on"
+            " the entity list.\n\nr0: Monster ID\nreturn: Pointer to the newly"
+            " initialized entity, or null if the entity couldn't be initialized"
+        ),
+    )
+
     SpawnTrap = Symbol(
         None,
         None,
         None,
         (
             "Spawns a trap on the floor. Fails if there are more than 64 traps already"
             " on the floor.\n\nThis modifies the appropriate fields on the dungeon"
@@ -15467,35 +15880,46 @@
             " items already on the floor.\n\nThis initializes a new entry in the entity"
             " table and points it to the corresponding slot in the item info"
             " list.\n\nr0: position\nreturn: entity pointer for the newly added item,"
             " or null on failure"
         ),
     )
 
-    ShouldDisplayEntityMessages = Symbol(
+    ShouldMinimapDisplayEntity = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if a given entity should be displayed on the minimap\n\nr0: Entity"
+            " pointer\nreturn: True if the entity should be displayed on the minimap"
+        ),
+    )
+
+    ShouldDisplayEntity = Symbol(
         None,
         None,
         None,
         (
-            "Checks if messages that involve a certain entity should be displayed or"
-            " suppressed.\n\nFor example, it returns false if the entity is an"
-            " invisible enemy.\n\nr0: Entity pointer\nr1: ?\nreturn: True if messages"
-            " involving the entity should be displayed, false if they should be"
-            " suppressed."
+            "Checks if an entity should be displayed or not.\n\nFor example, it returns"
+            " false if the entity is an invisible enemy.\nAlso used to determine if"
+            " messages that involve a certain entity should be displayed or"
+            " suppressed.\n\nr0: Entity pointer\nr1: (?) Seems to be 1 for monsters and"
+            " 0 for items.\nreturn: True if the entity and its associated messages"
+            " should be displayed, false if they shouldn't."
         ),
     )
 
-    ShouldDisplayEntityMessagesWrapper = Symbol(
+    ShouldDisplayEntityWrapper = Symbol(
         None,
         None,
         None,
         (
-            "Calls ShouldDisplayEntityMessages with r1 = 0\n\nr0: Entity"
-            " pointer\nreturn: True if messages involving the entity should be"
-            " displayed, false if they should be suppressed."
+            "Calls ShouldDisplayEntity with r1 = 0\n\nr0: Entity pointer\nreturn: True"
+            " if the entity and its associated messages should be displayed, false if"
+            " they shouldn't."
         ),
     )
 
     CanSeeTarget = Symbol(
         None,
         None,
         None,
@@ -15615,28 +16039,54 @@
         (
             "Returns dungeon::display_data::visibility_range. If the visibility range"
             " is 0, returns 2 instead.\n\nreturn: Visibility range of the current"
             " floor, or 2 if the visibility is 0."
         ),
     )
 
-    PlayEffectAnimation = Symbol(
+    PlayEffectAnimationEntity = Symbol(
         None,
         None,
         None,
         (
             "Just a guess. This appears to be paired often with"
             " GetEffectAnimationField0x19, and also has calls AnimationHasMoreFrames in"
             " a loop alongside AdvanceFrame(66) calls.\n\nThe third parameter skips the"
             " loop entirely. It seems like in this case the function might just preload"
-            " some animation frames for later use??\n\nr0: entity pointer\nr1: ?\nr2:"
-            " appears to be a flag for actually running the animation now? If this is"
-            " 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn: status"
-            " code, or maybe the number of frames or something? Either way, -1 seems to"
-            " indicate the animation being finished or something?"
+            " some animation frames for later use??\n\nr0: entity pointer\nr1: Effect"
+            " ID\nr2: appears to be a flag for actually running the animation now? If"
+            " this is 0, the AdvanceFrame loop is skipped entirely.\nothers: ?\nreturn:"
+            " status code, or maybe the number of frames or something? Either way, -1"
+            " seems to indicate the animation being finished or something?"
+        ),
+    )
+
+    PlayEffectAnimationPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Takes a position struct in r0 and converts it to a pixel position struct"
+            " before calling PlayEffectAnimationPixelPos\n\nr0: Position where the"
+            " effect should be played\nr1: Effect ID\nr2: Unknown flag (same as the one"
+            " in PlayEffectAnimationEntity)\nreturn: Result of call to"
+            " PlayEffectAnimationPixelPos"
+        ),
+    )
+
+    PlayEffectAnimationPixelPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Seems like a variant of PlayEffectAnimationEntity that uses pixel"
+            " coordinates as its first parameter instead of an entity pointer.\n\nr0:"
+            " Pixel position where the effect should be played\nr1: Effect ID\nr2:"
+            " Unknown flag (same as the one in PlayEffectAnimationEntity)\nreturn: Same"
+            " as PlayEffectAnimationEntity"
         ),
     )
 
     UpdateStatusIconFlags = Symbol(
         None,
         None,
         None,
@@ -15724,15 +16174,15 @@
         None,
         None,
         (
             "Copies all entries in the floor's monster spawn list that have a sprite"
             " size >= 6 to the specified buffer.\n\nThe parameter in r1 can be used to"
             " specify how many entries are already present in the buffer. Entries added"
             " by this function will be placed after those, and the total returned in r1"
-            " will account for existing entries as well.\n\nr0: (output) Buffer where"
+            " will account for existing entries as well.\n\nr0: [output] Buffer where"
             " the result will be stored\nr1: Current amount of entries in the"
             " buffer\nreturn: New amount of entries in the buffer"
         ),
     )
 
     IsOnMonsterSpawnList = Symbol(
         None,
@@ -16104,14 +16554,26 @@
             " the effect of the Switcher Orb). \n\nThe function checks for the Suction"
             " Cups ability for both the user and the target, and for the Mold Breaker"
             " ability on the user.\n\nr0: pointer to user entity\nr1: pointer to target"
             " entity"
         ),
     )
 
+    SetLeaderActionFields = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the leader's monster::action::action_id to the specified"
+            " value.\n\nAlso sets monster::action::action_use_idx and"
+            " monster::action::field_0xA to 0, as well as monster::action::field_0x10"
+            " and monster::action::field_0x12 to -1.\n\nr0: ID of the action to set"
+        ),
+    )
+
     ClearMonsterActionFields = Symbol(
         None,
         None,
         None,
         (
             "Clears the fields related to AI in the monster's data struct, setting them"
             " all to 0.\nSpecifically, monster::action::action_id,"
@@ -16191,14 +16653,27 @@
         (
             "Sets a monster's action to action::ACTION_REGULAR_ATTACK, with a specified"
             " direction.\n\nr0: Pointer to the monster's action field\nr1: Direction in"
             " which to use the move. Gets stored in monster::action::direction."
         ),
     )
 
+    SetActionUseMovePlayer = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets a monster's action to action::ACTION_USE_MOVE_PLAYER, with a"
+            " specified monster and move index.\n\nr0: Pointer to the monster's action"
+            " field\nr1: Index of the monster that is using the move on the entity"
+            " list. Gets stored in monster::action::action_use_idx.\nr2: Index of the"
+            " move to use (0-3). Gets stored in monster::action::field_0xA."
+        ),
+    )
+
     SetActionUseMoveAi = Symbol(
         None,
         None,
         None,
         (
             "Sets a monster's action to action::ACTION_USE_MOVE_AI, with a specified"
             " direction and move index.\n\nr0: Pointer to the monster's action"
@@ -16345,14 +16820,169 @@
             "If the flag for a trapper trap is set, handles spawning a trap based upon"
             " the\ninformation inside the dungeon struct. Uses the entity for logging a"
             " message\ndepending on success or failure.\n\nr0: entity pointer\nreturn:"
             " true if a trap was spawned succesfully"
         ),
     )
 
+    TryTriggerTrap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called whenever a monster steps on a trap.\n\nThe function will try to"
+            " trigger it. Nothing will happen if the pokémon has the same team as the"
+            " trap. The attempt to trigger the trap can also fail due to IQ skills, due"
+            " to the trap failing to work (random chance), etc.\n\nr0: Entity who"
+            " stepped on the trap\nr1: Trap position\nr2: ?\nr3: ?"
+        ),
+    )
+
+    ApplyMudTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly lowers attack, special attack, defense, or special defense of the"
+            " defender by 3 stages.\n\nr0: attacker entity pointer\nr1: defender entity"
+            " pointer"
+        ),
+    )
+
+    ApplyStickyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to make something in the bag"
+            " sticky. Otherwise, try to make the item the monster is holding"
+            " sticky.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyGrimyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, randomly try to turn food items in the"
+            " toolbox into\ngrimy food. Otherwise, try to make the food item the"
+            " monster is holding grimy food.\n\nr0: attacker entity pointer\nr1:"
+            " defender entity pointer"
+        ),
+    )
+
+    ApplyPitfallTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the defender is the leader, end the current floor unless it has a"
+            " rescue point.\nOtherwise, make the entity faint and ignore reviver seeds."
+            " If not called by a random\ntrap, break the grate on the pitfall"
+            " trap.\n\nr0: attacker entity pointer\nr1: defender entity pointer\nr2:"
+            " tile pointer\nr3: bool caused by random trap"
+        ),
+    )
+
+    ApplySummonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Randomly spawns 2-4 enemy monsters around the position. The entity is only"
+            " used for\nlogging messages.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyPpZeroTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the PP of one of the defender's moves to 0.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyPokemonTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Turns item in the same room as the tile at the position (usually just the"
+            " entities's\nposition) into monsters. If the position is in a hallway,"
+            " convert items in a 3x3 area\ncentered on the position into"
+            " monsters.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTripTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to drop the defender's item and places it on the floor.\n\nr0:"
+            " attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyToxicSpikesTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to inflict 10 damage on the defender and then tries to poison"
+            " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer"
+        ),
+    )
+
+    ApplyRandomTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Selects a random trap that isn't a wonder tile and isn't a random trap and"
+            " calls\nApplyTrapEffect on all monsters that is different from the trap's"
+            " team.\n\nr0: Triggered trap\nr1: User\nr2: Target, normally same as"
+            " user\nr3: Tile that contains the trap\nstack[0]: position"
+        ),
+    )
+
+    ApplyGrudgeTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Spawns several monsters around the position and gives all monsters on the"
+            " floor the\ngrudge status condition.\n\nr0: entity pointer\nr1: position"
+        ),
+    )
+
+    ApplyTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Performs the effect of a triggered trap.\n\nThe trap's animation happens"
+            " before this function is called.\n\nr0: Triggered trap\nr1: User\nr2:"
+            " Target, normally same as user\nr3: Tile that contains the trap\nstack[0]:"
+            " position\nstack[1]: trap ID\nstack[2]: bool caused by random"
+            " trap\nreturn: True if the trap should be destroyed after the effect is"
+            " applied"
+        ),
+    )
+
+    RevealTrapsNearby = Symbol(
+        None,
+        None,
+        None,
+        "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         (
             "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a"
             " function used during development to disable recruiting. If it returns"
@@ -16376,28 +17006,63 @@
         None,
         (
             "Returns a pointer to the action data of the current leader (field 0x4A on"
             " its monster struct).\n\nNo params."
         ),
     )
 
+    GetEntityTouchscreenArea = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the area on the touchscreen that contains the sprite of the"
+            " specified entity\n\nr0: Entity pointer\nr1: [output] struct where the"
+            " result should be written"
+        ),
+    )
+
     SetLeaderAction = Symbol(
         None,
         None,
         None,
         (
             "Sets the leader's action field depending on the inputs given by the"
             " player.\n\nThis function also accounts for other special situations that"
             " can force a certain action, such as when the leader is running. The"
             " function also takes care of opening the main menu when X is pressed.\nThe"
             " function generally doesn't return until the player has an action"
             " set.\n\nNo params."
         ),
     )
 
+    ShouldLeaderKeepRunning = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Determines if the leader should keep running. Returns false if the leader"
+            " bumps into something, or if an action that should stop the leader takes"
+            " place.\n\nreturn: True if the leader should keep running, false if it"
+            " should stop."
+        ),
+    )
+
+    CheckLeaderTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the tile the leader just stepped on and performs any required"
+            " actions, such as picking up items, triggering traps, etc.\n\nContains a"
+            " switch that checks the type of the tile the leader just stepped on.\n\nNo"
+            " params."
+        ),
+    )
+
     ChangeLeader = Symbol(
         None,
         None,
         None,
         (
             "Tries to change the current leader to the monster specified by"
             " dungeon::new_leader.\n\nAccounts for situations that can prevent changing"
@@ -16537,14 +17202,25 @@
         (
             "Handles a fainted pokémon (reviving does not count as fainting).\n\nr0:"
             " Fainted entity\nr1: Damage source (move ID or greater than the max move"
             " id for other causes)\nr2: Entity responsible of the fainting"
         ),
     )
 
+    MoveMonsterToPos = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Moves a monster to the target position. Used both for regular movement and"
+            " special movement (like teleportation).\n\nr0: Entity pointer\nr1: X"
+            " target position\nr2: Y target position\nr3: ?"
+        ),
+    )
+
     UpdateAiTargetPos = Symbol(
         None,
         None,
         None,
         (
             "Given a monster, updates its target_pos field based on its current"
             " position and the direction in which it plans to attack.\n\nr0: Entity"
@@ -16669,14 +17345,24 @@
             "Restores PP for all moves, clears flags move::f_consume_2_pp,"
             " move::flags2_unk5 and move::flags2_unk7, and sets flag"
             " move::f_consume_pp.\nCalled when a monster is revived.\n\nr0: pointer to"
             " entity whose moves will be restored"
         ),
     )
 
+    BoostIQ = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's IQ.\n\nr0: monster entity pointer\nr1: iq"
+            " boost\nr2: bool suppress logs"
+        ),
+    )
+
     ShouldMonsterHeadToStairs = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given monster should try to reach the stairs when controlled"
             " by the AI\n\nr0: Entity pointer\nreturn: True if the monster should try"
@@ -16693,14 +17379,28 @@
             " dungeon::mew_cannot_spawn or the second parameter are true.\n\nCalled"
             " before spawning an enemy, appears to be checking if Mew can spawn on the"
             " current floor.\n\nr0: monster id\nr1: return false if the monster id is"
             " Mew\nreturn: bool"
         ),
     )
 
+    TryEndStatusWithAbility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if any of the defender's active abilities would end one of their"
+            " current status\nconditions. For example, if the ability Own Tempo will"
+            " stop confusion.\n\nCalled after changing a monster's ability with skill"
+            " swap, role play, or trace to\nremove statuses the monster should no"
+            " longer be affected by.\n\nr0: attacker entity pointer\nr1: defender"
+            " entity pointer"
+        ),
+    )
+
     ExclusiveItemEffectIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is a team member under the effects of a certain"
             " exclusive item effect.\n\nr0: entity pointer\nr1: exclusive item effect"
@@ -16830,14 +17530,27 @@
             "Checks if a monster does not gain experience.\n\nThis basically just"
             " inverts IsSpecialStoryAlly, with the exception of also checking for the"
             " 'Joined At' field being DUNGEON_CLIENT (is this set for mission"
             " clients?).\n\nr0: monster pointer\nreturn: bool"
         ),
     )
 
+    InitOtherMonsterData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes stats, IQ skills and moves for a given monster\n\nMight only"
+            " be used when spawning fixed room monsters.\n\nr0: Entity pointer\nr1:"
+            " Fixed room monster stats index\nr2: Spawn direction? (when calling this"
+            " function while spawning a fixed room monster, this is the parameter value"
+            " associated to the spawn action, after converting it to a direction.)"
+        ),
+    )
+
     SpawnTeam = Symbol(
         None,
         None,
         None,
         "Seems to initialize and spawn the team when entering a dungeon.\n\nr0: ?",
     )
 
@@ -16881,16 +17594,28 @@
     )
 
     InitMonster = Symbol(
         None,
         None,
         None,
         (
-            "Initializes a monster struct.\n\nr0: pointer to monster to initialize\nr1:"
-            " some flag"
+            "Initializes the monster struct within the provided entity struct.\n\nr0:"
+            " ?\nr1: Pointer to the entity whose monster struct should be"
+            " initialized\nr2: pointer to the entity's spawned_monster_data struct\nr3:"
+            " (?) Pointer to something"
+        ),
+    )
+
+    SubInitMonster = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called by InitMonster. Initializes some fields on the monster"
+            " struct.\n\nr0: pointer to monster to initialize\nr1: some flag"
         ),
     )
 
     MarkShopkeeperSpawn = Symbol(
         None,
         None,
         None,
@@ -16995,14 +17720,24 @@
         (
             "Returns the number of attacks that a monster can do in one turn (1 or"
             " 2).\n\nChecks for the abilities Swift Swim, Chlorophyll, Unburden, and"
             " for exclusive items.\n\nr0: pointer to entity\nreturns: int"
         ),
     )
 
+    GetMonsterDisplayNameType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Determines how the name of a monster should be displayed.\n\nr0: Entity"
+            " pointer\nreturn: Display name type"
+        ),
+    )
+
     GetMonsterName = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: buffer\nr1: TargetInfo",
     )
 
@@ -17153,14 +17888,39 @@
         None,
         (
             "Checks if a monster has the sleep, nightmare, or napping status.\n\nr0:"
             " entity pointer\nreturn: bool"
         ),
     )
 
+    CanMonsterMoveInDirection = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the given monster can move in the specified direction\n\nReturns"
+            " false if any monster is standing on the target tile\n\nr0: Monster entity"
+            " pointer\nr1: Direction to check\nreturn: bool"
+        ),
+    )
+
+    GetFinalMobilityType = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the mobility type of a monster, after accounting for things that"
+            " could affect it (like items or IQ skills)\n\nIf the specified direction"
+            " is DIR_NONE, direction checks are skipped. If it's not,"
+            " MOBILITY_INTANGIBLE is only returned if the direction is not"
+            " diagonal.\n\nr0: Monster entity pointer\nr1: Base mobility type\nr2:"
+            " Direction of mobility\nreturn: Final mobility type"
+        ),
+    )
+
     IsMonsterCornered = Symbol(
         None,
         None,
         None,
         (
             "True if the given monster is cornered (it can't move in any"
             " direction)\n\nr0: Entity pointer\nreturn: True if the monster can't move"
@@ -17188,15 +17948,15 @@
         None,
         None,
         (
             "Checks whether an AI-controlled monster can move in the specified"
             " direction.\nAccounts for walls, other monsters on the target position and"
             " IQ skills that might prevent a monster from moving into a specific"
             " location, such as House Avoider, Trap Avoider or Lava Evader.\n\nr0:"
-            " Entity pointer\nr1: Direction\nr2: (output) True if movement was not"
+            " Entity pointer\nr1: Direction\nr2: [output] True if movement was not"
             " possible because there was another monster on the target tile, false"
             " otherwise.\nreturn: True if the monster can move in the specified"
             " direction, false otherwise."
         ),
     )
 
     ShouldMonsterRunAway = Symbol(
@@ -17216,14 +17976,47 @@
         (
             "Calls ShouldMonsterRunAway and returns its result. It also calls another"
             " function if the result was true.\n\nr0: Entity pointer\nr1: ?\nreturn:"
             " Result of the call to ShouldMonsterRunAway"
         ),
     )
 
+    SafeguardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is under the effect of Safeguard.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: flag to log a message\nreturn:"
+            " bool"
+        ),
+    )
+
+    LeafGuardIsActive = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is protected by the ability Leaf Guard.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer\nr2: flag to log a"
+            " message\nreturn: bool"
+        ),
+    )
+
+    IsProtectedFromStatDrops = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting their stats dropped"
+            " by the user.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     NoGastroAcidStatus = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster does not have the Gastro Acid status.\n\nr0: entity"
             " pointer\nreturn: bool"
@@ -17384,14 +18177,25 @@
             "Updates monster::state_flags and monster::prev_state_flags with new"
             " values.\n\nr0: monster pointer\nr1: bitmask for bits to update\nr2:"
             " whether to set the bits indicated by the mask to 1 or 0\nreturn: whether"
             " or not any of the masked bits changed from the previous state"
         ),
     )
 
+    IsProtectedFromNegativeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the target monster is protected from getting a negative status"
+            " condition.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " flag to log a message\nreturn: bool"
+        ),
+    )
+
     AddExpSpecial = Symbol(
         None,
         None,
         None,
         (
             "Adds to a monster's experience points, subject to experience boosting"
             " effects.\n\nThis function appears to be called only under special"
@@ -17405,17 +18209,31 @@
     )
 
     EnemyEvolution = Symbol(
         None,
         None,
         None,
         (
-            "Checks if the specified enemy should evolve because it just defeated an"
-            " ally, and if so, attempts to evolve it.\n\nr0: Pointer to the enemy to"
-            " check"
+            "Checks if any enemies on the floor should evolve and attempts to evolve"
+            " it. The\nentity pointer passed seems to get replaced by a generic"
+            " placeholder entity if the\nentity pointer passed is invalid.\n\nr0:"
+            " entity pointer"
+        ),
+    )
+
+    LevelUpItemEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to level up the the target. Calls LevelUp with a few extra checks"
+            " and messages\nfor using as an item. Used for the Joy Seed and Golden"
+            " Seed.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: number"
+            " of levels\nr3: bool message flag?\nstack[0]: bool show level up dialog"
+            " (for example 'Hey, I leveled up!' with a portrait)?"
         ),
     )
 
     TryDecreaseLevel = Symbol(
         None,
         None,
         None,
@@ -17427,27 +18245,31 @@
     )
 
     LevelUp = Symbol(
         None,
         None,
         None,
         (
-            "Note: unverified, ported from Irdkwia's notes\n\nr0: user entity"
-            " pointer\nr1: target entity pointer\nr2: message flag?\nr3: ?\nreturn:"
-            " success flag?"
+            "Attempts to level up the the target. Fails if the target's level can't be"
+            " raised. The show show level up dialog bool does nothing for monsters not"
+            " on the team.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " bool message flag?\nr3: bool show level up dialog (for example 'Hey, I"
+            " leveled up!' with a portrait)?\nreturn: success flag"
         ),
     )
 
     EvolveMonster = Symbol(
         None,
         None,
         None,
         (
-            "Makes the specified monster evolve into the specified species.\n\nr0:"
-            " Pointer to the entity to evolve\nr1: ?\nr2: Species to evolve into"
+            "Makes the specified monster evolve into the specified species. Has a"
+            " special case when\na monster evolves into Ninjask and tries to spawn a"
+            " Shedinja as well.\n\nr0: user entity pointer?\nr1: target pointer to the"
+            " entity to evolve\nr2: Species to evolve into"
         ),
     )
 
     GetSleepAnimationId = Symbol(
         None,
         None,
         None,
@@ -17469,14 +18291,58 @@
             " example, this delayed display system is used to display multiple monsters"
             " moving at once even though they take turns sequentially.\n\nr0: Pointer"
             " to an entity. Can be null.\nreturns: Seems to be true if there were any"
             " pending actions to display."
         ),
     )
 
+    CheckNonLeaderTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Similar to CheckLeaderTile, but for other monsters.\n\nUsed both for"
+            " enemies and team members.\n\nr0: Entity pointer"
+        ),
+    )
+
+    EndNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Cures the target's negative status conditions. The game rarely (if not"
+            " never) calls\nthis function with the bool to remove the wrapping status"
+            " false.\n\nr0: pointer to user\nr1: pointer to target\nr2: bool play"
+            " animation\nr3: bool log failure message\nstack[0]: bool remove wrapping"
+            " status\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    EndNegativeStatusConditionWrapper = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Calls EndNegativeStatusCondition with remove wrapping status false.\n\nr0:"
+            " pointer to user\nr1: pointer to target\nr2: bool play animation\nr3: bool"
+            " log failure message\nreturn: bool succesfully removed negative status"
+        ),
+    )
+
+    TransferNegativeStatusCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Transfers all negative status conditions the user has and gives then to"
+            " the target.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     EndSleepClassStatus = Symbol(
         None,
         None,
         None,
         (
             "Cures the target's sleep, sleepless, nightmare, yawn or napping status due"
             " to the action of the user, and prints the event to the log.\n\nr0:"
@@ -17582,14 +18448,25 @@
         (
             "Removes the target's magnet rise status due to the action of the user, and"
             " prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
             " target"
         ),
     )
 
+    TransferNegativeBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to transfer the the negative blinker class status conditions from"
+            " the user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer\nreturn: Whether or not the status could be transferred"
+        ),
+    )
+
     TryTriggerMonsterHouse = Symbol(
         None,
         None,
         None,
         (
             "Triggers a Monster House for an entity, if the right conditions are"
             " met.\n\nConditions: entity is valid and on the team, the tile is a"
@@ -18017,14 +18894,26 @@
         (
             "Inflicts the Sleep status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
             " number of turns\nr3: flag to log a message on failure"
         ),
     )
 
+    IsProtectedFromSleepClassStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the monster is immune to sleep class status conditions.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nr2: ignore safeguard\nr3:"
+            " ignore other protections (exclusive items + leaf guard)\nstack[0]: flag"
+            " to log a message on failure\nreturn: bool"
+        ),
+    )
+
     TryInflictNightmareStatus = Symbol(
         None,
         None,
         None,
         (
             "Inflicts the Nightmare status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
@@ -18527,91 +19416,638 @@
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
             " to log a message on failure\nr3: flag to only perform the check for"
             " inflicting without actually inflicting\nreturn: Whether or not the status"
             " could be inflicted"
         ),
     )
 
-    TryInflictDestinyBond = Symbol(
+    TryInflictDestinyBondStatus = Symbol(
         None,
         None,
         None,
         (
             "Inflicts the Destiny Bond status condition on a target monster if"
             " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
-    TryInvisify = Symbol(
+    TryInflictSureShotStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Sure Shot status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWhifferStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Whiffer status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSetDamageStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Set Damage status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictFocusEnergyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Focus Energy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictDecoyStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Decoy status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictCurseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Curse status condition on a target monster if possible and if"
+            " the user is\na ghost type. Otherwise, just boost the user's defense and"
+            " attack then lower the user's\nspeed.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
+    TryInflictSnatchStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Snatch status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictTauntStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Taunt status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictStockpileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Stockpile condition on a target monster if possible. Won't"
+            " boost the level\nof stockpiling above 3.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nreturn: Whether or not the status could be"
+            " inflicted or boosted"
+        ),
+    )
+
+    TryInflictInvisibleStatus = Symbol(
         None,
         None,
         None,
         (
             "Attempts to turn the target invisible.\n\nThe user pointer is only used"
             " when calling LogMessage functions.\n\nr0: user entity pointer\nr1: target"
             " entity pointer"
         ),
     )
 
+    TryInflictPerishSongStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Perish Song status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEncoreStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Encore status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryDecreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reduce the belly size of the target. Only when max belly shrink"
+            " is 0, the\ncurrent belly is reduced by belly to lose. If both are"
+            " non-zero, only the max belly\nshrink is applied.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: belly to lose\nr3: max belly"
+            " shrink"
+        ),
+    )
+
+    TryIncreaseBelly = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restore belly and possibly boost max belly of the target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2:"
+            " belly to restore\nr3: max belly boost (if belly is full)\nstack[0]: flag"
+            " to log a message"
+        ),
+    )
+
+    TryInflictMuzzledStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Muzzled status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
     TryTransform = Symbol(
         None,
         None,
         None,
         (
             "Attempts to transform the target into the species of a random monster"
             " contained in the list returned by MonsterSpawnListPartialCopy.\n\nThe"
             " user pointer is only used when calling LogMessage functions.\n\nr0: user"
             " entity pointer\nr1: target entity pointer"
         ),
     )
 
+    TryInflictMobileStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mobile status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictExposedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Exposed status condition on a target monster if possible."
+            " Only applies to\nGhost types and monsters with raised evasion. If the"
+            " animation effect ID is 0,\ndefaults to animation ID 0xE (this fallback"
+            " animation likely can't be seen in normal\nplay).\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: animation effect ID\nr3: flag to"
+            " only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryActivateIdentifyCondition = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the flag for the identify orb which causes monsters holding items to"
+            " be shown with\na blue exclamation mark status icon.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictBlinkerStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Blinker status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting\nr3:"
+            " flag to log a message on failure\nreturn: Whether or not the status could"
+            " be inflicted"
+        ),
+    )
+
     IsBlinded = Symbol(
         None,
         None,
         None,
         (
             "Returns true if the monster has the blinded status (see"
             " statuses::blinded), or if it is not the leader and is holding Y-Ray"
             " Specs.\n\nr0: pointer to entity\nr1: flag for whether to check for the"
             " held item\nreturn: bool"
         ),
     )
 
+    TryInflictCrossEyedStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Cross-Eyed status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually"
+            " inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictEyedropStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Eyedrop status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictSlipStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Slip status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer\nreturn: Whether or not"
+            " the status could be inflicted"
+        ),
+    )
+
+    TryInflictDropeyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Dropeye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nreturn:"
+            " Whether or not the status could be inflicted"
+        ),
+    )
+
     RestoreMovePP = Symbol(
         None,
         None,
         None,
         (
             "Restores the PP of all the target's moves by the specified amount.\n\nr0:"
             " user entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3:"
             " flag to suppress message logging"
         ),
     )
 
-    SetReflectDamageCountdownTo4 = Symbol(
+    ApplyProteinEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: attack boost"
+        ),
+    )
+
+    ApplyCalciumEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's special attack stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special attack boost"
+        ),
+    )
+
+    ApplyIronEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to boost the target's defense stat.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer\nr2: defense boost"
+        ),
+    )
+
+    ApplyZincEffect = Symbol(
         None,
         None,
         None,
         (
-            "Sets the monster's reflect damage countdown to a global value"
+            "Tries to boost the target's special defense stat.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: special defense boost"
+        ),
+    )
+
+    TryInflictLongTossStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Long Toss status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictPierceStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Pierce status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictGastroAcidStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Gastro Acid status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    SetAquaRingHealingCountdownTo4 = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the countdown for Aqua Ring healing countdown to a global value"
             " (0x4).\n\nr0: pointer to entity"
         ),
     )
 
+    ApplyAquaRingHealing = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Applies the passive healing gained from the Aqua Ring status.\n\nr0:"
+            " pointer to entity"
+        ),
+    )
+
+    TryInflictAquaRingStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Aqua Ring status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLuckyChantStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Lucky Chant status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictHealBlockStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Heal Block status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    MonsterHasEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns true if the monster has the Embargo status condition.\n\nr0:"
+            " pointer to entity\nreturn: bool"
+        ),
+    )
+
+    LogItemBlockedByEmbargo = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Logs the error message when the usage of an item is blocked by"
+            " Embargo.\n\nr0: pointer to entity"
+        ),
+    )
+
+    TryInflictEmbargoStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Embargo status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to log message\nr3: flag to only perform the check for inflicting without"
+            " actually inflicting\nreturn: Whether or not the status could be inflicted"
+        ),
+    )
+
+    TryInflictMiracleEyeStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Miracle Eye status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: flag"
+            " to only perform the check for inflicting without actually inflicting"
+        ),
+    )
+
+    TryInflictMagnetRiseStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magnet Rise status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
     HasConditionalGroundImmunity = Symbol(
         None,
         None,
         None,
         (
             "Checks if a monster is currently immune to Ground-type moves for reasons"
             " other than typing and ability.\n\nThis includes checks for Gravity and"
             " Magnet Rise.\n\nr0: entity pointer\nreturn: bool"
         ),
     )
 
+    TryInflictSafeguardStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Safeguard status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMistStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mist status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictWishStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Wish status condition on a target monster if possible.\n\nr0:"
+            " user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMagicCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Magic Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictLightScreenStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Light Screen status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictReflectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Reflect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Protect status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorCoatStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Coat status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictEndureStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Endure status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictMirrorMoveStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Mirror Move status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictConversion2Status = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Conversion2 status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryInflictVitalThrowStatus = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Inflicts the Vital Throw status condition on a target monster if"
+            " possible.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    TryResetStatChanges = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to reset the stat changes of the defender.\n\nr0: attacker entity"
+            " pointer\nr1: defender entity pointer\nr3: bool to force animation"
+        ),
+    )
+
     MirrorMoveIsActive = Symbol(
         None,
         None,
         None,
         (
             "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if"
             " the effects is a status, 2 if it comes from an exclusive item, 0"
@@ -18769,21 +20205,101 @@
         (
             "Seems to apply an item's effect via a giant switch statement?\n\nr3:"
             " attacker pointer\nstack[0]: defender pointer\nstack[1]: thrown item"
             " pointer\nothers: ?"
         ),
     )
 
-    ViolentSeedBoost = Symbol(
+    ApplyCheriBerryEffect = Symbol(
         None,
         None,
         None,
         (
-            "Applies the Violent Seed boost to an entity.\n\nr0: attacker pointer\nr1:"
-            " defender pointer"
+            "Tries to heal the paralysis status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyPechaBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the poisoned and badly poisoned status condition. Prints a"
+            " message on\nfailure.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyRawstBerryEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to heal the burn status condition. Prints a message on"
+            " failure.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyHungerSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Empties the targets belly to cause Hungry Pal status in non-leader"
+            " monsters and\nFamished in the leader monster.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyVileSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Reduces the targets defense and special defense stages to the lowest"
+            " level.\n\nr0: attacker pointer\nr1: defender pointer"
+        ),
+    )
+
+    ApplyViolentSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the target's offensive stats stages to the max.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGinsengEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Boosts the power of the move at the top of the target's Move List. Appears"
+            " to have a\nleftover check to boost the power of a move by 3 instead of 1"
+            " that always fails because\nthe chance is 0.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyBlastSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If thrown, unfreeze and deal fixed damage to the defender. If not thrown,"
+            " try to find \na monster in front of the attacker. If a monster is found"
+            " unfreeze and dedal fixed \ndamage to the defender. Appears to have a"
+            " leftover check for if the current fixed room is a boss fight and loads a"
+            " different pointer for the damage when used in a boss room.\nHowever, this"
+            " isn't noticeable because both the normal and boss damage is the"
+            " same.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: bool"
+            " thrown"
         ),
     )
 
     ApplyGummiBoostsDungeonMode = Symbol(
         None,
         None,
         None,
@@ -18825,14 +20341,68 @@
         None,
         (
             "If the target monster is a Linoone, restores all the PP of all the"
             " target's moves.\n\nr0: user entity pointer\nr1: target entity pointer"
         ),
     )
 
+    ApplyDoughSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target monster is a team member, set dough_seed_extra_poke_flag to"
+            " true to \nmake extra poke spawn on the next floor. Otherwise, do"
+            " nothing.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyViaSeedEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Tries to randomly teleport the target with a message for eating the"
+            " seed.\n\nr0: user entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGravelyrockEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Restores 10 hunger to the target and will raise the target's IQ if they"
+            " are a bonsly\nor sudowoodo.\n\nr0: user entity pointer\nr1: target entity"
+            " pointer"
+        ),
+    )
+
+    ApplyGonePebbleEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Causes a few visual effects, temporarily changes the dungeon music to the"
+            " Goodnight\ntrack, and gives the target the enduring status.\n\nr0: user"
+            " entity pointer\nr1: target entity pointer"
+        ),
+    )
+
+    ApplyGracideaEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "If the target is Shaymin, attempt to change the target's form to Shaymin"
+            " Sky Forme. Otherwise, do nothing.\n\nr0: user entity pointer\nr1: target"
+            " entity pointer"
+        ),
+    )
+
     ShouldTryEatItem = Symbol(
         None,
         None,
         None,
         (
             "Checks if a given item should be eaten by the TryEatItem"
             " effect.\n\nReturns false if the ID is lower than 0x45, greater than 0x8A"
@@ -18906,15 +20476,29 @@
         None,
         None,
         None,
         (
             "Creates an explosion if possible.\n\nThe target monster is considered the"
             " source of the explosion.\n\nr0: user entity pointer\nr1: target entity"
             " pointer\nr2: coordinates where the explosion should take place"
-            " (unverified)\nr3: ?\nstack[0]: ?\nstack[1]: damage source (normally"
+            " (center)\nr3: explosion radius (only works correctly with 1 and"
+            " 2)\nstack[0]: damage type\nstack[1]: damage source"
+        ),
+    )
+
+    TryAftermathExplosion = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Creates the explosion for the ability aftermath if possible.\n\nThe target"
+            " monster is considered the source of the explosion.\n\nr0: user entity"
+            " pointer\nr1: target entity pointer\nr2: coordinates where the explosion"
+            " should take place (center)\nr3: explosion radius (only works correctly"
+            " with 1 and 2)\nstack[0]: damage type\nstack[1]: damage source (normally"
             " DAMAGE_SOURCE_EXPLOSION)"
         ),
     )
 
     TryWarp = Symbol(
         None,
         None,
@@ -19382,14 +20966,57 @@
     GetStairsRoom = Symbol(
         None,
         None,
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    UpdateTrapsVisibility = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Exact purpose unknown. Gets called whenever a trap tile is shown or"
+            " hidden.\n\nNo params."
+        ),
+    )
+
+    DrawTileGrid = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Draws a grid on the nearby walkable tiles. Triggered by pressing Y.\n\nr0:"
+            " Coordinates of the entity around which the grid will be drawn\nr1: ?\nr2:"
+            " ?\nr3: ?"
+        ),
+    )
+
+    HideTileGrid = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Hides the grid on the nearby walkable tiles. Triggered by releasing"
+            " Y.\n\nNo params."
+        ),
+    )
+
+    DiscoverMinimap = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Discovers the tiles around the specified position on the minimap.\n\nThe"
+            " discovery radius depends on the visibility range of the floor. If"
+            " display_data::blinded is true, the function returns early without doing"
+            " anything.\n\nr0: Position around which the map should be discovered"
+        ),
+    )
+
     IsWaterTileset = Symbol(
         None,
         None,
         None,
         (
             "Returns flag tileset_property::is_water_tileset for the current"
             " tileset\n\nreturn: True if the current tileset is a water tileset"
@@ -19455,14 +21082,34 @@
         (
             "Sets the boost_kecleon_shop_spawn_chance field on the dungeon struct"
             " depending on if a team member has the exclusive item effect for more"
             " kecleon shops.\n\nNo params."
         ),
     )
 
+    SetDoughSeedFlag = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Sets the dough_seed_extra_money_flag field on the dungeon struct to the"
+            " given value.\n\nr0: bool to set the flag to"
+        ),
+    )
+
+    TrySpawnDoughSeedPoke = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks the dough_seed_extra_money_flag field on the dungeon struct and"
+            " tries to spawn\nextra poke if it is set.\n\nNo params."
+        ),
+    )
+
     IsSecretBazaar = Symbol(
         None,
         None,
         None,
         "Checks if the current floor is the Secret Bazaar.\n\nreturn: bool",
     )
 
@@ -19513,28 +21160,62 @@
         None,
         (
             "Checks if the current floor is a secret bazaar or a secret"
             " room.\n\nreturn: bool"
         ),
     )
 
+    HiddenStairsPresent = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Checks if the hidden stairs are present on this floor.\n\nThe function"
+            " checks that dungeon_generation_info::hidden_stairs_pos isn't (-1,"
+            " -1)\n\nreturn: True if the hidden stairs are present on this floor, false"
+            " otherwise."
+        ),
+    )
+
+    HiddenStairsTrigger = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Called whenever the leader steps on the hidden stairs.\n\nIf the stairs"
+            " hadn't been revealed yet, plays the corresponding animation.\n\nr0: True"
+            " to display a message if the stairs are revealed, false to omit it."
+        ),
+    )
+
     GetDungeonGenInfoUnk0C = Symbol(
         None, None, None, "return: dungeon_generation_info::field_0xc"
     )
 
     GetMinimapData = Symbol(
         None,
         None,
         None,
         (
             "Returns a pointer to the minimap_display_data struct in the dungeon"
             " struct.\n\nreturn: minimap_display_data*"
         ),
     )
 
+    DrawMinimapTile = Symbol(
+        None,
+        None,
+        None,
+        "Draws a single tile on the minimap.\n\nr0: X position\nr1: Y position",
+    )
+
+    UpdateMinimap = Symbol(
+        None, None, None, "Graphically updates the minimap\n\nNo params."
+    )
+
     SetMinimapDataE447 = Symbol(
         None,
         None,
         None,
         (
             "Sets minimap_display_data::field_0xE447 to the specified value\n\nr0:"
             " Value to set the field to"
@@ -19558,14 +21239,35 @@
         None,
         (
             "Sets minimap_display_data::field_0xE448 to the specified value\n\nr0:"
             " Value to set the field to"
         ),
     )
 
+    InitWeirdMinimapMatrix = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initializes the matrix at minimap_display_data+0xE000. Seems to overflow"
+            " said matrix when doing so.\n\nNo params."
+        ),
+    )
+
+    InitMinimapDisplayTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to initialize an instance of struct minimap_display_tile\n\nr0:"
+            " Pointer to struct to init\nr1: Seems to be a pointer to the file that"
+            " stores minimap icons or something like that"
+        ),
+    )
+
     LoadFixedRoomDataVeneer = Symbol(
         None,
         None,
         None,
         (
             "Likely a linker-generated veneer for LoadFixedRoomData.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nNo"
@@ -20257,14 +21959,24 @@
             " reached by the traversal algorithm, then the stairs must not be reachable"
             " from that tile.\n\nr0: x coordinate of the stairs\nr1: y coordinate of"
             " the stairs\nr2: flag to always return true, but set a special bit on all"
             " walkable tiles that aren't reachable from the stairs\nreturn: bool"
         ),
     )
 
+    GetNextFixedRoomAction = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Returns the next action that needs to be performed when spawning a fixed"
+            " room tile.\n\nreturn: Next action ID"
+        ),
+    )
+
     ConvertWallsToChasms = Symbol(
         None, None, None, "Converts all wall tiles to chasms.\n\nNo params."
     )
 
     ResetInnerBoundaryTileRows = Symbol(
         None,
         None,
@@ -20315,25 +22027,75 @@
             " HIDDEN_STAIRS_RANDOM_SECRET_BAZAAR_OR_SECRET_ROOM and the"
             " floor_properties::hidden_stairs_spawn_chance) into a concrete hidden"
             " stairs type.\n\nr0: dungeon generation info pointer\nr1: floor properties"
             " pointer\nreturn: enum hidden_stairs_type"
         ),
     )
 
+    GetFinalKecleonShopSpawnChance = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Gets the kecleon shop spawn chance for the floor.\n\nWhen"
+            " dungeon::boost_kecleon_shop_spawn_chance is false, returns the same value"
+            " as the input. When it's true, returns the input (chance * 1.2).\n\nr0:"
+            " base kecleon shop spawn chance,"
+            " floor_properties::kecleon_shop_spawn_chance\nreturn: int"
+        ),
+    )
+
     ResetHiddenStairsSpawn = Symbol(
         None,
         None,
         None,
         (
             "Resets hidden stairs spawn information for the floor. This includes the"
             " position on the floor generation status as well as the flag indicating"
             " whether the spawn was blocked.\n\nNo params."
         ),
     )
 
+    PlaceFixedRoomTile = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Used to spawn a single tile when generating a fixed room. The tile might"
+            " contain an item or a monster.\n\nr0: Pointer to the tile to spawn\nr1:"
+            " Fixed room action to perform. Controls what exactly will be spawned. The"
+            " action is actually 12 bits long, the highest 4 bits are used as a"
+            " parameter that represents a direction (for example, when spawning a"
+            " monster).\nr2: Tile X position\nr3: Tile Y position"
+        ),
+    )
+
+    FixedRoomActionParamToDirection = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Converts the parameter stored in a fixed room action value to a direction"
+            " ID.\n\nThe conversion is performed by subtracting 1 to the value. If the"
+            " parameter had a value of 0, DIR_NONE is returned.\n\nr0: Parameter"
+            " value\nreturn: Direction"
+        ),
+    )
+
+    ApplyKeyEffect = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Attempts to open a locked door in front of the target if a locked door has"
+            " not already\nbeen open on the floor.\n\nr0: user entity pointer\nr1:"
+            " target entity pointer"
+        ),
+    )
+
     LoadFixedRoomData = Symbol(
         None,
         None,
         None,
         (
             "Loads fixed room data from BALANCE/fixed.bin into the buffer pointed to by"
             " FIXED_ROOM_DATA_PTR.\n\nNo params."
@@ -21107,15 +22869,27 @@
             " (if the corresponding parameter was set).\n\nr0: ID of the string to"
             " display\nr1: True to wait for player input before closing the dialogue"
             " box, false to close it automatically once all the characters get"
             " printed.\nr2: ? (r0 in DisplayMessage)\nr3: ?\nstack[0]: ?\nstack[1]: ?"
         ),
     )
 
-    OpenMenu = Symbol(None, None, None, "Note: unverified, ported from Irdkwia's notes")
+    OpenMenu = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Opens a menu. The menu to open depends on the specified parameter.\n\nIt"
+            " looks like the function takes a parameter in r0, but doesn't use it. r1"
+            " doesn't even get set when this function is called.\n\nr0: (?) Unused by"
+            " the function. Seems to be 1 byte long.\nr1: (?) Unused by the function."
+            " Seems to be 1 byte long.\nr2: True to open the bag menu, false to open"
+            " the main dungeon menu"
+        ),
+    )
 
     OthersMenuLoop = Symbol(
         None,
         None,
         None,
         (
             "Called on each frame while the in-dungeon 'others' menu is open.\n\nIt"
@@ -21290,27 +23064,27 @@
         None,
         (
             "The move target and range code for special healing moves that target just"
             " the user (0x273).\n\ntype: struct move_target_and_range (+ padding)"
         ),
     )
 
-    PLAIN_SEED_VALUE = Symbol(
-        None, None, None, "Some value related to the Plain Seed (0xBE9)."
+    PLAIN_SEED_STRING_ID = Symbol(
+        None, None, None, "The string ID for eating a Plain Seed (0xBE9)."
     )
 
     MAX_ELIXIR_PP_RESTORATION = Symbol(
         None,
         None,
         None,
         "The amount of PP restored per move by ingesting a Max Elixir (0x3E7).",
     )
 
-    SLIP_SEED_VALUE = Symbol(
-        None, None, None, "Some value related to the Slip Seed (0xC75)."
+    SLIP_SEED_FAIL_STRING_ID = Symbol(
+        None, None, None, "The string ID for when eating the Slip Seed fails (0xC75)."
     )
 
     ROCK_WRECKER_MOVE_ID = Symbol(
         None, None, None, "The move ID for Rock Wrecker (453)."
     )
 
     CASTFORM_NORMAL_FORM_MALE_ID = Symbol(
@@ -22055,15 +23829,28 @@
     loadaddress = None
     length = None
     functions = NaItcmOverlay3Functions
     data = NaItcmOverlay3Data
 
 
 class NaItcmOverlay30Functions:
-    pass
+    WriteQuicksaveData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Function responsible for writing dungeon data when quicksaving.\n\nAmong"
+            " other things, it contains a loop that goes through all the monsters in"
+            " the current dungeon, copying their data to the buffer. The data is not"
+            " copied as-is though, the game uses a reduced version of the monster"
+            " struct containing only the minimum required data to resume the game"
+            " later.\n\nr0: Pointer to buffer where data should be written\nr1: Buffer"
+            " size. Seems to be 0x5800 (22 KB) when the function is called."
+        ),
+    )
 
 
 class NaItcmOverlay30Data:
     OVERLAY30_JP_STRING_1 = Symbol(None, None, None, "みさき様")
 
     OVERLAY30_JP_STRING_2 = Symbol(None, None, None, "やよい様")
```

## pmdsky_debug_py/protocol.py

```diff
@@ -547,14 +547,19 @@
     ]
 
     LoadFileInPack: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetDungeonResultMsg: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetDamageSource: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetItemCategoryVeneer: Symbol[
         Optional[List[int]],
@@ -592,14 +597,19 @@
     ]
 
     IsAuraBow: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    IsTreasureBox: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     InitItem: Symbol[
         Optional[List[int]],
         None,
     ]
 
     InitStandardItem: Symbol[
         Optional[List[int]],
@@ -747,15 +757,15 @@
     ]
 
     GetItemMoveId: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    TestItemFlag0xE: Symbol[
+    TestItemAiFlag: Symbol[
         Optional[List[int]],
         None,
     ]
 
     IsItemInTimeDarkness: Symbol[
         Optional[List[int]],
         None,
@@ -777,14 +787,19 @@
     ]
 
     SetMoneyCarried: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    AddMoneyCarried: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetCurrentBagCapacity: Symbol[
         Optional[List[int]],
         None,
     ]
 
     IsBagFull: Symbol[
         Optional[List[int]],
@@ -942,14 +957,19 @@
     ]
 
     ScriptSpecialProcess0x39: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    CountNbItemsOfTypeInStorage: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     CountItemTypeInStorage: Symbol[
         Optional[List[int]],
         None,
     ]
 
     RemoveItemsTypeInStorage: Symbol[
         Optional[List[int]],
@@ -1487,29 +1507,49 @@
     ]
 
     DeleteWanTableEntry: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    AllocateWanTableEntry: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     FindWanTableEntry: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetLoadedWanTableEntry: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    InitWanTable: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     LoadWanTableEntry: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    LoadWanTableEntryFromPack: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    LoadWanTableEntryFromPackUseProvidedMemory: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ReplaceWanFromBinFile: Symbol[
         Optional[List[int]],
         None,
     ]
 
     DeleteWanTableEntryVeneer: Symbol[
         Optional[List[int]],
@@ -1637,14 +1677,19 @@
     ]
 
     SetStringPower: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetDungeonResultString: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SetQuestionMarks: Symbol[
         Optional[List[int]],
         None,
     ]
 
     StrcpySimple: Symbol[
         Optional[List[int]],
@@ -2027,14 +2072,19 @@
     ]
 
     GetSpecialEpisodeType: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetExecuteSpecialEpisodeType: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     HasPlayedOldGame: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetPerformanceFlagWithChecks: Symbol[
         Optional[List[int]],
@@ -2062,15 +2112,15 @@
     ]
 
     SetDungeonConquest: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    CheckDungeonOpen: Symbol[
+    GetDungeonMode: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GlobalProgressAlloc: Symbol[
         Optional[List[int]],
         None,
@@ -2187,14 +2237,34 @@
     ]
 
     LoadPortrait: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    SetEnterDungeon: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    InitDungeonInit: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    IsNoLossPenaltyDungeon: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    CheckMissionRestrictions: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetNbFloors: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetNbFloorsPlusOne: Symbol[
         Optional[List[int]],
@@ -2217,14 +2287,39 @@
     ]
 
     DungeonFloorToGroupFloor: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetMissionRank: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetOutlawLevel: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetOutlawLeaderLevel: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetOutlawMinionLevel: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    AddGuestMonster: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetGroundNameId: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SetAdventureLogStructLocation: Symbol[
         Optional[List[int]],
@@ -2847,14 +2942,19 @@
     ]
 
     LoadM2nAndN2m: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GuestMonsterToGroundMonster: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     StrcmpMonsterName: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetLvlStats: Symbol[
         Optional[List[int]],
@@ -3352,14 +3452,19 @@
     ]
 
     DungeonSwapIdxToId: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetDungeonModeSpecial: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ResumeBgm: Symbol[
         Optional[List[int]],
         None,
     ]
 
     FlushChannels: Symbol[
         Optional[List[int]],
@@ -3367,14 +3472,49 @@
     ]
 
     UpdateChannels: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ClearIrqFlag: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    EnableIrqFlag: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    SetIrqFlag: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    EnableIrqFiqFlags: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    SetIrqFiqFlags: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetIrqFlag: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    WaitForever2: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     WaitForInterrupt: Symbol[
         Optional[List[int]],
         None,
     ]
 
     FileInit: Symbol[
         Optional[List[int]],
@@ -7036,14 +7176,19 @@
     ]
 
     AIR_BLADE_DAMAGE_MULTIPLIER: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    KECLEON_SHOP_BOOST_CHANCE_MULTIPLIER: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     HIDDEN_STAIRS_SPAWN_CHANCE_MULTIPLIER: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     YAWN_TURN_RANGE: Symbol[
         Optional[List[int]],
@@ -7450,14 +7595,19 @@
     ]
 
     SprintfStatic: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetExclusiveItemRequirements: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     StatusUpdate: Symbol[
         Optional[List[int]],
         None,
     ]
 
 
 class Overlay11DataProtocol(Protocol):
@@ -7542,14 +7692,19 @@
     ]
 
     GROUND_STATE_MAP: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GROUND_STATE_WEATHER: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GROUND_STATE_PTRS: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
 
 Overlay11Protocol = SectionProtocol[
@@ -9480,35 +9635,65 @@
     ]
 
     FadeToBlack: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    CheckTouchscreenArea: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetTrapInfo: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetItemInfo: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetTileAtEntity: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    UpdateEntityPixelPos: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    CreateEnemyEntity: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SpawnTrap: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SpawnItemEntity: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    ShouldDisplayEntityMessages: Symbol[
+    ShouldMinimapDisplayEntity: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ShouldDisplayEntity: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    ShouldDisplayEntityMessagesWrapper: Symbol[
+    ShouldDisplayEntityWrapper: Symbol[
         Optional[List[int]],
         None,
     ]
 
     CanSeeTarget: Symbol[
         Optional[List[int]],
         None,
@@ -9555,15 +9740,25 @@
     ]
 
     GetVisibilityRange: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    PlayEffectAnimation: Symbol[
+    PlayEffectAnimationEntity: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    PlayEffectAnimationPos: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    PlayEffectAnimationPixelPos: Symbol[
         Optional[List[int]],
         None,
     ]
 
     UpdateStatusIconFlags: Symbol[
         Optional[List[int]],
         None,
@@ -9750,14 +9945,19 @@
     ]
 
     TrySwitchPlace: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    SetLeaderActionFields: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ClearMonsterActionFields: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SetMonsterActionFields: Symbol[
         Optional[List[int]],
@@ -9785,14 +9985,19 @@
     ]
 
     SetActionRegularAttack: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    SetActionUseMovePlayer: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SetActionUseMoveAi: Symbol[
         Optional[List[int]],
         None,
     ]
 
     RunFractionalTurn: Symbol[
         Optional[List[int]],
@@ -9850,14 +10055,84 @@
     ]
 
     TrySpawnTrapperTrap: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryTriggerTrap: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyMudTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyStickyTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyGrimyTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyPitfallTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplySummonTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyPpZeroTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyPokemonTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyTripTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyToxicSpikesTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyRandomTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyGrudgeTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    RevealTrapsNearby: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     DebugRecruitingEnabled: Symbol[
         Optional[List[int]],
         None,
     ]
 
     IsSecretBazaarNpcBehavior: Symbol[
         Optional[List[int]],
@@ -9865,19 +10140,34 @@
     ]
 
     GetLeaderAction: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetEntityTouchscreenArea: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SetLeaderAction: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ShouldLeaderKeepRunning: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    CheckLeaderTile: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ChangeLeader: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ResetDamageData: Symbol[
         Optional[List[int]],
@@ -9945,14 +10235,19 @@
     ]
 
     HandleFaint: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    MoveMonsterToPos: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     UpdateAiTargetPos: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SetMonsterTypeAndAbility: Symbol[
         Optional[List[int]],
@@ -10005,24 +10300,34 @@
     ]
 
     RestorePpAllMovesSetFlags: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    BoostIQ: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ShouldMonsterHeadToStairs: Symbol[
         Optional[List[int]],
         None,
     ]
 
     MewSpawnCheck: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryEndStatusWithAbility: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ExclusiveItemEffectIsActive: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetTeamMemberWithIqSkill: Symbol[
         Optional[List[int]],
@@ -10075,14 +10380,19 @@
     ]
 
     IsExperienceLocked: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    InitOtherMonsterData: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SpawnTeam: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SpawnInitialMonsters: Symbol[
         Optional[List[int]],
@@ -10100,14 +10410,19 @@
     ]
 
     InitMonster: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    SubInitMonster: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     MarkShopkeeperSpawn: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SpawnShopkeepers: Symbol[
         Optional[List[int]],
@@ -10145,14 +10460,19 @@
     ]
 
     GetNumberOfAttacks: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetMonsterDisplayNameType: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetMonsterName: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SprintfStatic: Symbol[
         Optional[List[int]],
@@ -10215,14 +10535,24 @@
     ]
 
     IsMonsterSleeping: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    CanMonsterMoveInDirection: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetFinalMobilityType: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsMonsterCornered: Symbol[
         Optional[List[int]],
         None,
     ]
 
     CanAttackInDirection: Symbol[
         Optional[List[int]],
@@ -10240,14 +10570,29 @@
     ]
 
     ShouldMonsterRunAwayVariation: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    SafeguardIsActive: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    LeafGuardIsActive: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    IsProtectedFromStatDrops: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     NoGastroAcidStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
     AbilityIsActive: Symbol[
         Optional[List[int]],
@@ -10315,24 +10660,34 @@
     ]
 
     UpdateStateFlags: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    IsProtectedFromNegativeStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     AddExpSpecial: Symbol[
         Optional[List[int]],
         None,
     ]
 
     EnemyEvolution: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    LevelUpItemEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TryDecreaseLevel: Symbol[
         Optional[List[int]],
         None,
     ]
 
     LevelUp: Symbol[
         Optional[List[int]],
@@ -10350,14 +10705,34 @@
     ]
 
     DisplayActions: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    CheckNonLeaderTile: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    EndNegativeStatusCondition: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    EndNegativeStatusConditionWrapper: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TransferNegativeStatusCondition: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     EndSleepClassStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
     EndBurnClassStatus: Symbol[
         Optional[List[int]],
@@ -10400,14 +10775,19 @@
     ]
 
     EndMagnetRiseStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TransferNegativeBlinkerClassStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TryTriggerMonsterHouse: Symbol[
         Optional[List[int]],
         None,
     ]
 
     RunMonsterAi: Symbol[
         Optional[List[int]],
@@ -10560,14 +10940,19 @@
     ]
 
     TryInflictSleepStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    IsProtectedFromSleepClassStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TryInflictNightmareStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryInflictNappingStatus: Symbol[
         Optional[List[int]],
@@ -10780,49 +11165,304 @@
     ]
 
     TryInflictLeechSeedStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    TryInflictDestinyBond: Symbol[
+    TryInflictDestinyBondStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictSureShotStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictWhifferStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictSetDamageStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictFocusEnergyStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictDecoyStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictCurseStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictSnatchStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictTauntStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictStockpileStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictInvisibleStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictPerishSongStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictEncoreStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryDecreaseBelly: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryIncreaseBelly: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    TryInvisify: Symbol[
+    TryInflictMuzzledStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryTransform: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryInflictMobileStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictExposedStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryActivateIdentifyCondition: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictBlinkerStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsBlinded: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryInflictCrossEyedStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictEyedropStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictSlipStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictDropeyeStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     RestoreMovePP: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    SetReflectDamageCountdownTo4: Symbol[
+    ApplyProteinEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyCalciumEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyIronEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyZincEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictLongTossStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictPierceStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictGastroAcidStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    SetAquaRingHealingCountdownTo4: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyAquaRingHealing: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictAquaRingStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictLuckyChantStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictHealBlockStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    MonsterHasEmbargoStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    LogItemBlockedByEmbargo: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictEmbargoStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictMiracleEyeStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictMagnetRiseStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
     HasConditionalGroundImmunity: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryInflictSafeguardStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictMistStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictWishStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictMagicCoatStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictLightScreenStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictReflectStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictProtectStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictMirrorCoatStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictEndureStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictMirrorMoveStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictConversion2Status: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictVitalThrowStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryResetStatChanges: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     MirrorMoveIsActive: Symbol[
         Optional[List[int]],
         None,
     ]
 
     Conversion2IsActive: Symbol[
         Optional[List[int]],
@@ -10880,15 +11520,50 @@
     ]
 
     ApplyItemEffect: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    ViolentSeedBoost: Symbol[
+    ApplyCheriBerryEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyPechaBerryEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyRawstBerryEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyHungerSeedEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyVileSeedEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyViolentSeedEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyGinsengEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyBlastSeedEffect: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ApplyGummiBoostsDungeonMode: Symbol[
         Optional[List[int]],
         None,
@@ -10905,14 +11580,39 @@
     ]
 
     ApplyMixElixirEffect: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ApplyDoughSeedEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyViaSeedEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyGravelyrockEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyGonePebbleEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyGracideaEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ShouldTryEatItem: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetMaxPpWrapper: Symbol[
         Optional[List[int]],
@@ -10945,14 +11645,19 @@
     ]
 
     TryExplosion: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryAftermathExplosion: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TryWarp: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryActivateNondamagingDefenderAbility: Symbol[
         Optional[List[int]],
@@ -11145,14 +11850,34 @@
     ]
 
     GetStairsRoom: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    UpdateTrapsVisibility: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    DrawTileGrid: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    HideTileGrid: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    DiscoverMinimap: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsWaterTileset: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetRandomSpawnMonsterID: Symbol[
         Optional[List[int]],
@@ -11185,14 +11910,24 @@
     ]
 
     UpdateShouldBoostKecleonShopSpawnChance: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    SetDoughSeedFlag: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TrySpawnDoughSeedPoke: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsSecretBazaar: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ShouldBoostHiddenStairsSpawnChance: Symbol[
         Optional[List[int]],
@@ -11215,24 +11950,44 @@
     ]
 
     IsSecretFloor: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    HiddenStairsPresent: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    HiddenStairsTrigger: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetDungeonGenInfoUnk0C: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetMinimapData: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    DrawMinimapTile: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    UpdateMinimap: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SetMinimapDataE447: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetMinimapDataE447: Symbol[
         Optional[List[int]],
@@ -11240,14 +11995,24 @@
     ]
 
     SetMinimapDataE448: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    InitWeirdMinimapMatrix: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    InitMinimapDisplayTile: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     LoadFixedRoomDataVeneer: Symbol[
         Optional[List[int]],
         None,
     ]
 
     IsNormalFloor: Symbol[
         Optional[List[int]],
@@ -11495,14 +12260,19 @@
     ]
 
     StairsAlwaysReachable: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetNextFixedRoomAction: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ConvertWallsToChasms: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ResetInnerBoundaryTileRows: Symbol[
         Optional[List[int]],
@@ -11520,19 +12290,39 @@
     ]
 
     GetHiddenStairsType: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetFinalKecleonShopSpawnChance: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ResetHiddenStairsSpawn: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    PlaceFixedRoomTile: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    FixedRoomActionParamToDirection: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ApplyKeyEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     LoadFixedRoomData: Symbol[
         Optional[List[int]],
         None,
     ]
 
     LoadFixedRoom: Symbol[
         Optional[List[int]],
@@ -12022,25 +12812,25 @@
     ]
 
     MOVE_TARGET_AND_RANGE_SPECIAL_USER_HEALING: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
-    PLAIN_SEED_VALUE: Symbol[
+    PLAIN_SEED_STRING_ID: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     MAX_ELIXIR_PP_RESTORATION: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
-    SLIP_SEED_VALUE: Symbol[
+    SLIP_SEED_FAIL_STRING_ID: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     ROCK_WRECKER_MOVE_ID: Symbol[
         Optional[List[int]],
         Optional[int],
@@ -12416,15 +13206,18 @@
     Overlay3FunctionsProtocol,
     Overlay3DataProtocol,
     Optional[int],
 ]
 
 
 class Overlay30FunctionsProtocol(Protocol):
-    pass
+    WriteQuicksaveData: Symbol[
+        Optional[List[int]],
+        None,
+    ]
 
 
 class Overlay30DataProtocol(Protocol):
     OVERLAY30_JP_STRING_1: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
```

## Comparing `pmdsky_debug_py-5.1.9.dist-info/METADATA` & `pmdsky_debug_py-6.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 5.1.9
+Version: 6.0.0
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

