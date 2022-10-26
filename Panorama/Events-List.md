---
title: Events List
description: List of all Panorama events
published: true
date: 2022-10-26T07:22:38.295Z
tags: engine, reference, panorama, scripting
editor: markdown
dateCreated: 2022-10-26T07:22:38.295Z
---

# Available Panorama Events

Generated using `dump_panorama_events markdown`.


| Event | Panel Event | Description | Can dispatch | Can listen for |
|---|---|---|---|---|
| `AddItemToCart(js_raw_arg itemID)` | No | Add an itemid to tournament store shopping cart | Yes | Yes |
| `AddStyle(string class)` | Yes | Add a CSS class to a panel. | Yes | Yes |
| `AddStyleToEachChild(string class)` | Yes | Add a CSS class to all children of this panel. | Yes | Yes |
| `AsyncEvent(float delay, event eventToFire)` | No | Fire another event after a delay (in seconds). | Yes | No |
| `CapabilityPopupIsOpen(js_raw_arg bActive)` | No | User is using the name tag or opening a case, or stickering.  Using one of the capabilites | Yes | Yes |
| `ChaosHudProcessInput()` | No | Fired when visible every tick or every other tick if the panel allows it. | Yes | Yes |
| `ChaosHudThink()` | No | Fired every tick or every other tick if the panel allows it. | Yes | Yes |
| `CloseAcceptPopup()` | No | Fired when accept match popup Closes. | Yes | Yes |
| `CloseSubMenuContent(js_raw_arg no args)` | No | Closes up the submenu panel | Yes | Yes |
| `DbgTestHudVote(string string: test type)` | No | Internal testing event. | Yes | Yes |
| `DemoPlaybackControl(string string, float float)` | No | Control demo playback | Yes | Yes |
| `DropInputFocus()` | Yes | Drop focus entirely from the window containing this panel. | Yes | Yes |
| `EndOfMatch_GetFreeForAllPlayerPosition_Response(js_raw_arg position)` | No | Callback for Scoreboard_GetFreeForAllPlayerPosition | Yes | Yes |
| `EndOfMatch_GetFreeForAllTopThreePlayers_Response(js_raw_arg first, js_raw_arg second, js_raw_arg third)` | No | Callback for Scoreboard_GetFreeForAllTopThreePlayers | Yes | Yes |
| `EndOfMatch_ShowNext()` | No | Notify the EndOfMatch controller to proceed to the next panel. | Yes | Yes |
| `FriendInvitedFromContextMenu(js_raw_arg xuid)` | No | invite friend from the playercard. Make the invite anim snow immediately instead of waiting for the callback that can take a long time. | Yes | Yes |
| `HideContentPanel(js_raw_arg no args)` | No | Hide all the content panels and show the default home dashboard | Yes | Yes |
| `HideSelectItemForCapabilityPopup()` | No | Hide this popup in inventory | Yes | Yes |
| `IfHasClassEvent(string class, event eventToFire)` | Yes | Fire another event if this panel has a given class. | Yes | No |
| `IfHoverOtherEvent(string otherPanelID, event eventToFire)` | Yes | Fire another event if currently hovering over a panel with the given ID. | Yes | No |
| `IfNotHasClassEvent(string class, event eventToFire)` | Yes | Fire another event if this panel does not have a given class. | Yes | No |
| `IfNotHoverOtherEvent(string otherPanelID, event eventToFire)` | Yes | Fire another event if not currently hovering over a panel with the given ID. | Yes | No |
| `InitAvatar(js_raw_arg xuid, js_raw_arg type of panel)` | No | Update the avatar panel data for a xuid | Yes | Yes |
| `InitializeTournamentsPage(js_raw_arg tournament ID)` | No | Loads the layout for a given tournament for active tournament tab | Yes | Yes |
| `InventoryItemPreview(js_raw_arg itemId)` | No | Just itemid | Yes | Yes |
| `LayoutReloaded()` | No | Called when a panel has its layout reloaded. | Yes | Yes |
| `LootlistItemPreview(js_raw_arg itemId)` | No | typeParams | Yes | Yes |
| `MainMenuTabShown(js_raw_arg tabid)` | No | Alert main menu tabs when they are shown, in case there is a data update needed | Yes | Yes |
| `MovePanelDown(int32 repeatCount)` | Yes | Move down from the panel. By default, this will change the focus position, but other panel types may implement this differently. | Yes | Yes |
| `MovePanelLeft(int32 repeatCount)` | Yes | Move left from the panel. By default, this will change the focus position, but other panel types may implement this differently. | Yes | Yes |
| `MovePanelRight(int32 repeatCount)` | Yes | Move right from the panel. By default, this will change the focus position, but other panel types may implement this differently. | Yes | Yes |
| `MovePanelUp(int32 repeatCount)` | Yes | Move up from the panel. By default, this will change the focus position, but other panel types may implement this differently. | Yes | Yes |
| `NavigateToTab(js_raw_arg tab name, js_raw_arg xml name, js_raw_arg If its a tab, js_raw_arg if you should add to stack)` | No | Closes up the submenu panel | Yes | Yes |
| `OpenInventory(js_raw_arg no args)` | No | opens the inventory menu from anywhere. | Yes | Yes |
| `OpenPlayMenu(js_raw_arg no args)` | No | opens the play menu from anywhere. EXAMPLE from party menu settings button from client | Yes | Yes |
| `OpenSidebarPanel(js_raw_arg no args)` | No | open the sidebar from a abutton click from anywhere | Yes | Yes |
| `OpenWatchMenu(js_raw_arg no args)` | No | opens the watch menu from anywhere. | Yes | Yes |
| `PageDown()` | No | Scroll the panel down by one page. | Yes | Yes |
| `PageLeft()` | No | Scroll the panel left by one page. | Yes | Yes |
| `PagePanelDown()` | Yes | Scroll the panel down by one page. | Yes | Yes |
| `PagePanelLeft()` | Yes | Scroll the panel left by one page. | Yes | Yes |
| `PagePanelRight()` | Yes | Scroll the panel left by one page. | Yes | Yes |
| `PagePanelUp()` | Yes | Scroll the panel up by one page. | Yes | Yes |
| `PageRight()` | No | Scroll the panel right by one page. | Yes | Yes |
| `PageUp()` | No | Scroll the panel up by one page. | Yes | Yes |
| `PanoramaCastVoteNo()` | Yes | Cast a NO vote for the currently active vote issue | Yes | Yes |
| `PanoramaCastVoteYes()` | Yes | Cast a YES vote for the currently active vote issue | Yes | Yes |
| `PanoramaGameTimeJumpEvent(float time jump delta in seconds)` | No | Fired when game time jump occurs usually for replay jumping back in time. | Yes | Yes |
| `RefreshActiveInventoryList()` | No | Make the active list get the items in it | Yes | Yes |
| `RefreshPickemPage(js_raw_arg tournament ID)` | No | refreshed pickem data | Yes | Yes |
| `RemoveItemFromCart(js_raw_arg itemID)` | No | Remove an item of this id from the tournament store shopping cart | Yes | Yes |
| `RemoveStyle(string class)` | Yes | Remove a CSS class from a panel. | Yes | Yes |
| `RemoveStyleFromEachChild(string class)` | Yes | Remove a CSS class from all children of this panel. | Yes | Yes |
| `Scoreboard_CycleStats()` | No | Cycle the stats. | Yes | Yes |
| `Scoreboard_GetFreeForAllPlayerPosition(js_raw_arg xuid)` | No | Given a player index and an xuid, returns top three players on that player's team | Yes | Yes |
| `Scoreboard_GetFreeForAllTopThreePlayers()` | No | Returns top three players on team 'ANY' | Yes | Yes |
| `Scoreboard_SetMuteAbusive(js_raw_arg newVal)` | No | set cl_mute_frequent_abusers | Yes | Yes |
| `Scoreboard_UnborrowMusicKit()` | No | Cancel Music Kit borrowing | Yes | Yes |
| `ScrollDown()` | No | Scroll the panel down by one line. | Yes | Yes |
| `ScrollLeft()` | No | Scroll the panel left by one line. | Yes | Yes |
| `ScrollPanelDown()` | Yes | Scroll the panel down by one line. | Yes | Yes |
| `ScrollPanelLeft()` | Yes | Scroll the panel left by one line. | Yes | Yes |
| `ScrollPanelRight()` | Yes | Scroll the panel right by one line. | Yes | Yes |
| `ScrollPanelUp()` | Yes | Scroll the panel up by one line. | Yes | Yes |
| `ScrollRight()` | No | Scroll the panel right by one line. | Yes | Yes |
| `ScrollToBottom()` | Yes | Scroll this panel to the bottom. | Yes | Yes |
| `ScrollToTop()` | Yes | Scroll this panel to the top. | Yes | Yes |
| `ScrollUp()` | No | Scroll the panel up by one line. | Yes | Yes |
| `SetChildPanelsSelected(bool selected)` | Yes | Set whether any child panels are :selected. | Yes | Yes |
| `SetInputFocus()` | Yes | Set focus to this panel. | Yes | Yes |
| `SetPanelEnabled(bool enabled)` | Yes | Sets whether the given panel is enabled | Yes | Yes |
| `SetPanelSelected(bool selected)` | Yes | Set whether this panel is :selected. | Yes | Yes |
| `ShowAcceptPopup(js_raw_arg popup)` | No | Fired when accept match popup is shown. | Yes | Yes |
| `ShowAcknowledgePopup(js_raw_arg updatetype, js_raw_arg itemid)` | No | show acknowledge popup, also takes params for when an item is updated but does not need to be acknowledged like after using a nametag | Yes | Yes |
| `ShowActiveTournamentPage(js_raw_arg tab to show id)` | No | Opens active tournament page in the watch panel | Yes | Yes |
| `ShowCenterPrintText(string utf8 message string, CCenterPrint::EPriority)` | No | Display the string in the center of the hud. | No | Yes |
| `ShowContentPanel(js_raw_arg no args)` | No | Show a content panel | Yes | Yes |
| `ShowDeleteItemConfirmationPopup(js_raw_arg itemid)` | No | When a user is trying to delete an item from inventory | Yes | Yes |
| `ShowLoadoutForItem(js_raw_arg slot)` | No | subslot | Yes | Yes |
| `ShowResetMusicVolumePopup(js_raw_arg itemid)` | No | When a user is trying to equip a musickit but has thier music volume off from inventory | Yes | Yes |
| `ShowSelectItemForCapabilityPopup(js_raw_arg capability, js_raw_arg itemid, js_raw_arg itemid2)` | No | Show popup in Inventory that allow you to select a second item for a capability that requires 2 items | Yes | Yes |
| `ShowTournamentStore()` | No | Show tournament store popup | Yes | Yes |
| `ShowTradeUpPanel()` | No | Show trade up panel | Yes | Yes |
| `ShowUseItemOnceConfirmationPopup(js_raw_arg itemid)` | No | When a user is trying to use an item from inventory that can be used once | Yes | Yes |
| `ShowVoteContextMenu()` | No | Show vote context menu in pause menu | Yes | Yes |
| `SidebarContextMenuActive(js_raw_arg bActive)` | No | Let the sidebar panel know if a context menu is active on a section of it. | Yes | Yes |
| `SidebarIsCollapsed(js_raw_arg bActive)` | No | Is sidebar collapsed. | Yes | Yes |
| `StartDecodeableAnim(js_raw_arg no args)` | No | tells the decode panel to play the animation | Yes | Yes |
| `StaticHudMenu_EntrySelected(panorama::CPanel2D * Panel representing the selected entry)` | No | Fired when any of the entries is activated | No | Yes |
| `StreamPanelClosed()` | No | Notify that user has closed stream panel | Yes | Yes |
| `SwitchStyle(string slot, string class)` | Yes | Switch which class the panel has for a given attribute slot. Allows easily changing between multiple states. | Yes | Yes |
| `TogglePanelSelected()` | Yes | Toggle whether this panel is :selected. | Yes | Yes |
| `ToggleStyle(string class)` | Yes | Toggle whether a panel has the given CSS class. | Yes | Yes |
| `TriggerStyle(string class)` | Yes | Remove then immediately add back a CSS class from a panel. Useful to re-trigger events like animations or sound effects. | Yes | Yes |
| `UpdateTradeUpPanel()` | No | Update trade up panel | Yes | Yes |
| `UpdateVanityModelData(js_raw_arg no args)` | No | Update the vanity model with list of anims and model panel from updated settings | Yes | Yes |
