---
title: JS API List
description: List of all Panorama JS APIs
published: true
date: 2022-10-26T07:21:01.929Z
tags: engine, reference, panorama, scripting
editor: markdown
dateCreated: 2022-10-26T07:21:01.929Z
---

# Available Panorama JS Methods and Properties

Generated using `dump_panorama_js_scopes markdown` in-game.

## $

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'length' | 'int32' | X | $.persistentStorage.length.  Returns an integer representing the number of data items stored in the Storage object. |

| Method Name | Signature | Description |
|---|---|---|
| `AsyncWebRequest` | `void $.AsyncWebRequest( js_raw_arg  )` | Make a web request |
| `CancelScheduled` | `void $.CancelScheduled( js_raw_arg  )` | Cancelse a scheduled function |
| `clear` | `void $.clear()` | $.persistentStorage.clear().  When invoked, will empty all keys out of the storage. |
| `CompressString` | `void $.CompressString( js_raw_arg  )` | $.CompressString(str). Compresses the given string, and encodes result in base64. |
| `CreatePanel` | `void $.CreatePanel( js_raw_arg  )` | Create a new panel |
| `DbgIsReloadingScript` | `void $.DbgIsReloadingScript( js_raw_arg  )` | Call during JS startup code to check if script is being reloaded |
| `DecompressString` | `void $.DecompressString( js_raw_arg  )` | $.DecompressString(str). Decompresses the given base64 encoded input into a string. |
| `DefineEvent` | `void $.DefineEvent( js_raw_arg  )` | Define an event |
| `DefinePanelEvent` | `void $.DefinePanelEvent( js_raw_arg  )` | Define an panel event |
| `DispatchEvent` | `void $.DispatchEvent( js_raw_arg  )` | Dispatch an event |
| `DispatchEventAsync` | `void $.DispatchEventAsync( js_raw_arg  )` | Dispatch an event to occur later |
| `Each` | `void $.Each( js_raw_arg  )` | Call a function on each given item |
| `FindChildInContext` | `void $.FindChildInContext( js_raw_arg  )` | Find an element |
| `GetContextPanel` | `void $.GetContextPanel( js_raw_arg  )` | Get the current panel context |
| `getItem` | `cstring $.getItem( cstring keyName )` | $.persistentStorage.getItem(keyName).  When passed a key name, will return that key's value. |
| `HTMLEscape` | `void $.HTMLEscape( js_raw_arg  )` | $.HTMLEscape(str, truncate=false).  Converts str, which must be 2048 utf-8 bytes or shorter, into an HTML-safe version.  If truncate=true, too long strings will be truncated instead of throwing an exception |
| `key` | `cstring $.key( int32 n )` | $.persistentStorage.key(n).  When passed a number n, this method will return the name of the nth key in the storage. |
| `Language` | `void $.Language( js_raw_arg  )` | Get the current language |
| `LoadKeyValuesFile` | `void $.LoadKeyValuesFile( js_raw_arg  )` | Load a named key values file and return as JS object |
| `Localize` | `void $.Localize( js_raw_arg  )` | Localize a string |
| `LocalizeSafe` | `void $.LocalizeSafe( js_raw_arg  )` | Localize a string, but return empty string if the localization token is not found |
| `Msg` | `void $.Msg( js_raw_arg  )` | Log a message |
| `PlaySoundEvent` | `void $.PlaySoundEvent( js_raw_arg  )` | $.PlaySoundEvent(str).  Plays the named sound event. |
| `RegisterEventHandler` | `void $.RegisterEventHandler( js_raw_arg  )` | Register an event handler |
| `RegisterForUnhandledEvent` | `void $.RegisterForUnhandledEvent( js_raw_arg  )` | Register a handler for an event that is not otherwise handled |
| `RegisterKeyBind` | `void $.RegisterKeyBind( string panelOrInputContext, string keys, callback )` | Register a key binding. `panelOrInputContext` is the panel or input context to bind on, this may be empty string if the binding is global. `keys` is a comma separated list of keys to bind. |
| `removeItem` | `void $.removeItem( cstring keyName )` | $.persistentStorage.removeItem(keyName).  When passed a key name, will remove that key from the storage. |
| `Schedule` | `void $.Schedule( js_raw_arg  )` | Schedule a function to be called later |
| `setItem` | `void $.setItem( cstring keyName, cstring keyValue )` | $.persistentStorage.setItem(keyName, keyValue).  When passed a key name and value, will add that key to the storage, or update that key's value if it already exists. |
| `StopSoundEvent` | `void $.StopSoundEvent( js_raw_arg  )` | $.StopSoundEvent(guid, [fadetime]). Stops the sound event. guid was returned from a previous call to PlaySoundEvent. fadetime is optional. |
| `UnregisterEventHandler` | `void $.UnregisterEventHandler( js_raw_arg  )` | Remove an event handler |
| `UnregisterForUnhandledEvent` | `void $.UnregisterForUnhandledEvent( js_raw_arg  )` | Remove an unhandled event handler |
| `UrlDecode` | `void $.UrlDecode( js_raw_arg  )` | $.UrlDecode(str).  Decodes str, which must be 2048 utf-8 bytes or shorter, from URL-encoded form. |
| `UrlEncode` | `void $.UrlEncode( js_raw_arg  )` | $.UrlEncode(str).  Encodes str, which must be 2048 utf-8 bytes or shorter, into URL-encoded form. |
| `Warning` | `void $.Warning( js_raw_arg  )` | Log a warning |
## Button

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool Button.AcceptsFocus()` |  |
| `AcceptsInput` | `bool Button.AcceptsInput()` |  |
| `AddClass` | `void Button.AddClass( cstring  )` |  |
| `ApplyStyles` | `void Button.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool Button.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool Button.CanSeeInParentScroll()` |  |
| `Children` | `unknown Button.Children()` |  |
| `ClearPanelEvent` | `void Button.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void Button.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool Button.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown Button.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void Button.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void Button.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void Button.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown Button.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown Button.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown Button.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown Button.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 Button.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring Button.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 Button.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown Button.GetChild( int32  )` |  |
| `GetChildCount` | `int32 Button.GetChildCount()` |  |
| `GetChildIndex` | `int32 Button.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown Button.GetFirstChild()` |  |
| `GetLastChild` | `unknown Button.GetLastChild()` |  |
| `GetParent` | `unknown Button.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown Button.GetPositionWithinWindow()` |  |
| `HasClass` | `bool Button.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool Button.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool Button.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool Button.HasKeyFocus()` |  |
| `IsDraggable` | `bool Button.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool Button.IsReadyForDisplay()` |  |
| `IsSelected` | `bool Button.IsSelected()` |  |
| `IsTransparent` | `bool Button.IsTransparent()` |  |
| `LoadLayout` | `bool Button.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void Button.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void Button.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void Button.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool Button.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void Button.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void Button.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void Button.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void Button.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void Button.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool Button.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void Button.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void Button.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void Button.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void Button.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void Button.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void Button.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void Button.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void Button.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void Button.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void Button.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void Button.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void Button.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void Button.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void Button.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void Button.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void Button.SetDraggable( bool  )` |  |
| `SetFocus` | `bool Button.SetFocus()` |  |
| `SetHasClass` | `void Button.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void Button.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void Button.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void Button.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void Button.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void Button.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void Button.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetTopOfInputContext` | `void Button.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void Button.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void Button.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void Button.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void Button.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void Button.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool Button.UpdateFocusInContext()` |  |
## ChaosBackbufferImagePanel

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool ChaosBackbufferImagePanel.AcceptsFocus()` |  |
| `AcceptsInput` | `bool ChaosBackbufferImagePanel.AcceptsInput()` |  |
| `AddClass` | `void ChaosBackbufferImagePanel.AddClass( cstring  )` |  |
| `ApplyStyles` | `void ChaosBackbufferImagePanel.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool ChaosBackbufferImagePanel.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool ChaosBackbufferImagePanel.CanSeeInParentScroll()` |  |
| `Children` | `unknown ChaosBackbufferImagePanel.Children()` |  |
| `ClearPanelEvent` | `void ChaosBackbufferImagePanel.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void ChaosBackbufferImagePanel.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool ChaosBackbufferImagePanel.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown ChaosBackbufferImagePanel.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void ChaosBackbufferImagePanel.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void ChaosBackbufferImagePanel.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void ChaosBackbufferImagePanel.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown ChaosBackbufferImagePanel.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown ChaosBackbufferImagePanel.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown ChaosBackbufferImagePanel.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown ChaosBackbufferImagePanel.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 ChaosBackbufferImagePanel.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring ChaosBackbufferImagePanel.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 ChaosBackbufferImagePanel.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown ChaosBackbufferImagePanel.GetChild( int32  )` |  |
| `GetChildCount` | `int32 ChaosBackbufferImagePanel.GetChildCount()` |  |
| `GetChildIndex` | `int32 ChaosBackbufferImagePanel.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown ChaosBackbufferImagePanel.GetFirstChild()` |  |
| `GetLastChild` | `unknown ChaosBackbufferImagePanel.GetLastChild()` |  |
| `GetParent` | `unknown ChaosBackbufferImagePanel.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown ChaosBackbufferImagePanel.GetPositionWithinWindow()` |  |
| `HasClass` | `bool ChaosBackbufferImagePanel.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool ChaosBackbufferImagePanel.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool ChaosBackbufferImagePanel.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool ChaosBackbufferImagePanel.HasKeyFocus()` |  |
| `IsDraggable` | `bool ChaosBackbufferImagePanel.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool ChaosBackbufferImagePanel.IsReadyForDisplay()` |  |
| `IsSelected` | `bool ChaosBackbufferImagePanel.IsSelected()` |  |
| `IsTransparent` | `bool ChaosBackbufferImagePanel.IsTransparent()` |  |
| `LoadLayout` | `bool ChaosBackbufferImagePanel.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void ChaosBackbufferImagePanel.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void ChaosBackbufferImagePanel.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void ChaosBackbufferImagePanel.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool ChaosBackbufferImagePanel.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void ChaosBackbufferImagePanel.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void ChaosBackbufferImagePanel.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void ChaosBackbufferImagePanel.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void ChaosBackbufferImagePanel.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void ChaosBackbufferImagePanel.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool ChaosBackbufferImagePanel.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void ChaosBackbufferImagePanel.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void ChaosBackbufferImagePanel.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void ChaosBackbufferImagePanel.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void ChaosBackbufferImagePanel.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void ChaosBackbufferImagePanel.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void ChaosBackbufferImagePanel.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void ChaosBackbufferImagePanel.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void ChaosBackbufferImagePanel.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void ChaosBackbufferImagePanel.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void ChaosBackbufferImagePanel.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void ChaosBackbufferImagePanel.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void ChaosBackbufferImagePanel.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void ChaosBackbufferImagePanel.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void ChaosBackbufferImagePanel.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void ChaosBackbufferImagePanel.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void ChaosBackbufferImagePanel.SetDraggable( bool  )` |  |
| `SetFocus` | `bool ChaosBackbufferImagePanel.SetFocus()` |  |
| `SetHasClass` | `void ChaosBackbufferImagePanel.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void ChaosBackbufferImagePanel.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void ChaosBackbufferImagePanel.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void ChaosBackbufferImagePanel.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void ChaosBackbufferImagePanel.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void ChaosBackbufferImagePanel.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void ChaosBackbufferImagePanel.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetTopOfInputContext` | `void ChaosBackbufferImagePanel.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void ChaosBackbufferImagePanel.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void ChaosBackbufferImagePanel.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void ChaosBackbufferImagePanel.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void ChaosBackbufferImagePanel.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void ChaosBackbufferImagePanel.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool ChaosBackbufferImagePanel.UpdateFocusInContext()` |  |
## ChaosMainMenu

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool ChaosMainMenu.AcceptsFocus()` |  |
| `AcceptsInput` | `bool ChaosMainMenu.AcceptsInput()` |  |
| `AddClass` | `void ChaosMainMenu.AddClass( cstring  )` |  |
| `ApplyStyles` | `void ChaosMainMenu.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool ChaosMainMenu.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool ChaosMainMenu.CanSeeInParentScroll()` |  |
| `Children` | `unknown ChaosMainMenu.Children()` |  |
| `ClearPanelEvent` | `void ChaosMainMenu.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void ChaosMainMenu.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool ChaosMainMenu.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown ChaosMainMenu.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void ChaosMainMenu.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void ChaosMainMenu.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void ChaosMainMenu.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown ChaosMainMenu.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown ChaosMainMenu.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown ChaosMainMenu.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown ChaosMainMenu.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 ChaosMainMenu.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring ChaosMainMenu.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 ChaosMainMenu.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown ChaosMainMenu.GetChild( int32  )` |  |
| `GetChildCount` | `int32 ChaosMainMenu.GetChildCount()` |  |
| `GetChildIndex` | `int32 ChaosMainMenu.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown ChaosMainMenu.GetFirstChild()` |  |
| `GetLastChild` | `unknown ChaosMainMenu.GetLastChild()` |  |
| `GetParent` | `unknown ChaosMainMenu.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown ChaosMainMenu.GetPositionWithinWindow()` |  |
| `HasClass` | `bool ChaosMainMenu.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool ChaosMainMenu.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool ChaosMainMenu.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool ChaosMainMenu.HasKeyFocus()` |  |
| `IsDraggable` | `bool ChaosMainMenu.IsDraggable()` |  |
| `IsMultiplayer` | `bool ChaosMainMenu.IsMultiplayer()` |  |
| `IsReadyForDisplay` | `bool ChaosMainMenu.IsReadyForDisplay()` |  |
| `IsSelected` | `bool ChaosMainMenu.IsSelected()` |  |
| `IsTransparent` | `bool ChaosMainMenu.IsTransparent()` |  |
| `LoadLayout` | `bool ChaosMainMenu.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void ChaosMainMenu.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void ChaosMainMenu.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void ChaosMainMenu.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool ChaosMainMenu.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void ChaosMainMenu.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void ChaosMainMenu.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void ChaosMainMenu.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void ChaosMainMenu.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void ChaosMainMenu.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool ChaosMainMenu.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void ChaosMainMenu.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void ChaosMainMenu.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void ChaosMainMenu.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void ChaosMainMenu.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void ChaosMainMenu.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void ChaosMainMenu.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void ChaosMainMenu.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void ChaosMainMenu.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void ChaosMainMenu.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void ChaosMainMenu.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void ChaosMainMenu.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void ChaosMainMenu.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void ChaosMainMenu.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void ChaosMainMenu.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void ChaosMainMenu.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void ChaosMainMenu.SetDraggable( bool  )` |  |
| `SetFocus` | `bool ChaosMainMenu.SetFocus()` |  |
| `SetHasClass` | `void ChaosMainMenu.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void ChaosMainMenu.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void ChaosMainMenu.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void ChaosMainMenu.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void ChaosMainMenu.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void ChaosMainMenu.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void ChaosMainMenu.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetTopOfInputContext` | `void ChaosMainMenu.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void ChaosMainMenu.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void ChaosMainMenu.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void ChaosMainMenu.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void ChaosMainMenu.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void ChaosMainMenu.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool ChaosMainMenu.UpdateFocusInContext()` |  |
## ChaosSettingsSlider

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'convar' | 'cstring' |   |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'max' | 'float' |   |  |
| 'min' | 'float' |   |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'value' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool ChaosSettingsSlider.AcceptsFocus()` |  |
| `AcceptsInput` | `bool ChaosSettingsSlider.AcceptsInput()` |  |
| `ActualValue` | `float ChaosSettingsSlider.ActualValue()` |  |
| `AddClass` | `void ChaosSettingsSlider.AddClass( cstring  )` |  |
| `ApplyStyles` | `void ChaosSettingsSlider.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool ChaosSettingsSlider.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool ChaosSettingsSlider.CanSeeInParentScroll()` |  |
| `Children` | `unknown ChaosSettingsSlider.Children()` |  |
| `ClearPanelEvent` | `void ChaosSettingsSlider.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void ChaosSettingsSlider.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool ChaosSettingsSlider.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown ChaosSettingsSlider.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void ChaosSettingsSlider.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void ChaosSettingsSlider.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void ChaosSettingsSlider.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown ChaosSettingsSlider.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown ChaosSettingsSlider.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown ChaosSettingsSlider.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown ChaosSettingsSlider.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 ChaosSettingsSlider.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring ChaosSettingsSlider.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 ChaosSettingsSlider.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown ChaosSettingsSlider.GetChild( int32  )` |  |
| `GetChildCount` | `int32 ChaosSettingsSlider.GetChildCount()` |  |
| `GetChildIndex` | `int32 ChaosSettingsSlider.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown ChaosSettingsSlider.GetFirstChild()` |  |
| `GetLastChild` | `unknown ChaosSettingsSlider.GetLastChild()` |  |
| `GetParent` | `unknown ChaosSettingsSlider.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown ChaosSettingsSlider.GetPositionWithinWindow()` |  |
| `HasClass` | `bool ChaosSettingsSlider.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool ChaosSettingsSlider.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool ChaosSettingsSlider.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool ChaosSettingsSlider.HasKeyFocus()` |  |
| `IsDraggable` | `bool ChaosSettingsSlider.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool ChaosSettingsSlider.IsReadyForDisplay()` |  |
| `IsSelected` | `bool ChaosSettingsSlider.IsSelected()` |  |
| `IsTransparent` | `bool ChaosSettingsSlider.IsTransparent()` |  |
| `LoadLayout` | `bool ChaosSettingsSlider.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void ChaosSettingsSlider.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void ChaosSettingsSlider.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void ChaosSettingsSlider.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool ChaosSettingsSlider.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void ChaosSettingsSlider.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void ChaosSettingsSlider.MoveChildBefore( unknown , unknown  )` |  |
| `OnShow` | `void ChaosSettingsSlider.OnShow()` |  |
| `RegisterForReadyEvents` | `void ChaosSettingsSlider.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void ChaosSettingsSlider.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void ChaosSettingsSlider.RemoveClass( cstring  )` |  |
| `RestoreCVarDefault` | `void ChaosSettingsSlider.RestoreCVarDefault()` |  |
| `ScrollParentToFitWhenFocused` | `bool ChaosSettingsSlider.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void ChaosSettingsSlider.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void ChaosSettingsSlider.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void ChaosSettingsSlider.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void ChaosSettingsSlider.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void ChaosSettingsSlider.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void ChaosSettingsSlider.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void ChaosSettingsSlider.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void ChaosSettingsSlider.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void ChaosSettingsSlider.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void ChaosSettingsSlider.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void ChaosSettingsSlider.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void ChaosSettingsSlider.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void ChaosSettingsSlider.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void ChaosSettingsSlider.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void ChaosSettingsSlider.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void ChaosSettingsSlider.SetDraggable( bool  )` |  |
| `SetFocus` | `bool ChaosSettingsSlider.SetFocus()` |  |
| `SetHasClass` | `void ChaosSettingsSlider.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void ChaosSettingsSlider.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void ChaosSettingsSlider.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void ChaosSettingsSlider.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void ChaosSettingsSlider.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void ChaosSettingsSlider.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void ChaosSettingsSlider.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetTopOfInputContext` | `void ChaosSettingsSlider.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void ChaosSettingsSlider.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void ChaosSettingsSlider.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void ChaosSettingsSlider.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void ChaosSettingsSlider.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void ChaosSettingsSlider.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool ChaosSettingsSlider.UpdateFocusInContext()` |  |
## Frame

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool Frame.AcceptsFocus()` |  |
| `AcceptsInput` | `bool Frame.AcceptsInput()` |  |
| `AddClass` | `void Frame.AddClass( cstring  )` |  |
| `ApplyStyles` | `void Frame.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool Frame.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool Frame.CanSeeInParentScroll()` |  |
| `Children` | `unknown Frame.Children()` |  |
| `ClearPanelEvent` | `void Frame.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void Frame.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool Frame.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown Frame.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void Frame.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void Frame.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void Frame.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown Frame.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown Frame.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown Frame.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown Frame.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 Frame.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring Frame.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 Frame.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown Frame.GetChild( int32  )` |  |
| `GetChildCount` | `int32 Frame.GetChildCount()` |  |
| `GetChildIndex` | `int32 Frame.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown Frame.GetFirstChild()` |  |
| `GetLastChild` | `unknown Frame.GetLastChild()` |  |
| `GetParent` | `unknown Frame.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown Frame.GetPositionWithinWindow()` |  |
| `HasClass` | `bool Frame.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool Frame.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool Frame.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool Frame.HasKeyFocus()` |  |
| `IsDraggable` | `bool Frame.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool Frame.IsReadyForDisplay()` |  |
| `IsSelected` | `bool Frame.IsSelected()` |  |
| `IsTransparent` | `bool Frame.IsTransparent()` |  |
| `LoadLayout` | `bool Frame.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void Frame.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void Frame.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void Frame.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool Frame.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void Frame.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void Frame.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void Frame.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void Frame.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void Frame.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool Frame.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void Frame.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void Frame.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void Frame.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void Frame.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void Frame.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void Frame.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void Frame.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void Frame.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void Frame.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void Frame.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void Frame.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void Frame.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void Frame.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void Frame.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void Frame.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void Frame.SetDraggable( bool  )` |  |
| `SetFocus` | `bool Frame.SetFocus()` |  |
| `SetHasClass` | `void Frame.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void Frame.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void Frame.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void Frame.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void Frame.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void Frame.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void Frame.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetSnippet` | `void Frame.SetSnippet( cstring  )` |  |
| `SetSource` | `void Frame.SetSource( cstring  )` |  |
| `SetTopOfInputContext` | `void Frame.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void Frame.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void Frame.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void Frame.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void Frame.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void Frame.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool Frame.UpdateFocusInContext()` |  |
## FriendsAPI

| Method Name | Signature | Description |
|---|---|---|
| `GetLocalPlayerName` | `cstring FriendsAPI.GetLocalPlayerName()` | Gets the name of the local player |
| `GetNameForXUID` | `cstring FriendsAPI.GetNameForXUID( uint64 xuid )` | Gets the name of the player with the given XUID. This will only be known by the local user if the given user is in their friends list, on the same game server, in a chat room or lobby, or in a small group with the local user |
## GameInterfaceAPI

| Method Name | Signature | Description |
|---|---|---|
| `ConsoleCommand` | `void GameInterfaceAPI.ConsoleCommand( cstring command )` | Executes the specified console command. |
| `GetGameUIState` | `int32 GameInterfaceAPI.GetGameUIState()` | Gets the current GameUI state. |
| `GetSettingBool` | `bool GameInterfaceAPI.GetSettingBool( cstring convar )` | Executes a lookup for the bool setting of the specified convar. |
| `GetSettingColor` | `unknown GameInterfaceAPI.GetSettingColor( cstring convar )` | Executes a lookup for the color setting of the specified convar. |
| `GetSettingFloat` | `float GameInterfaceAPI.GetSettingFloat( cstring convar )` | Executes a lookup for the float setting of the specified convar. |
| `GetSettingInt` | `int32 GameInterfaceAPI.GetSettingInt( cstring convar )` | Executes a lookup for the integer setting of the specified convar. |
| `GetSettingString` | `cstring GameInterfaceAPI.GetSettingString( cstring convar )` | Executes a lookup for the string setting of the specified convar. Can be null. |
| `RegisterGameEventHandler` | `uint32 GameInterfaceAPI.RegisterGameEventHandler( cstring event_name, unknown callback )` | Registers a callback for a specific game event type, returns an event handler ID to unregister with |
| `SetSettingBool` | `void GameInterfaceAPI.SetSettingBool( cstring convar, bool value )` | Executes a lookup for the specified convar and sets it to specified value. |
| `SetSettingColor` | `void GameInterfaceAPI.SetSettingColor( cstring convar, unknown value )` | Executes a lookup for the specified convar and sets it to specified value. |
| `SetSettingFloat` | `void GameInterfaceAPI.SetSettingFloat( cstring convar, float value )` | Executes a lookup for the specified convar and sets it to specified value. |
| `SetSettingInt` | `void GameInterfaceAPI.SetSettingInt( cstring convar, int32 value )` | Executes a lookup for the specified convar and sets it to specified value. |
| `SetSettingString` | `void GameInterfaceAPI.SetSettingString( cstring convar, cstring value )` | Executes a lookup for the specified convar and sets it to specified value. |
| `UnregisterGameEventHandler` | `void GameInterfaceAPI.UnregisterGameEventHandler( uint32 callback_id )` | Unregisters a previously registered event handler for a game event |
## Image

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool Image.AcceptsFocus()` |  |
| `AcceptsInput` | `bool Image.AcceptsInput()` |  |
| `AddClass` | `void Image.AddClass( cstring  )` |  |
| `ApplyStyles` | `void Image.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool Image.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool Image.CanSeeInParentScroll()` |  |
| `Children` | `unknown Image.Children()` |  |
| `ClearPanelEvent` | `void Image.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void Image.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool Image.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown Image.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void Image.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void Image.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void Image.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown Image.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown Image.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown Image.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown Image.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 Image.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring Image.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 Image.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown Image.GetChild( int32  )` |  |
| `GetChildCount` | `int32 Image.GetChildCount()` |  |
| `GetChildIndex` | `int32 Image.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown Image.GetFirstChild()` |  |
| `GetLastChild` | `unknown Image.GetLastChild()` |  |
| `GetParent` | `unknown Image.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown Image.GetPositionWithinWindow()` |  |
| `HasClass` | `bool Image.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool Image.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool Image.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool Image.HasKeyFocus()` |  |
| `IsDraggable` | `bool Image.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool Image.IsReadyForDisplay()` |  |
| `IsSelected` | `bool Image.IsSelected()` |  |
| `IsTransparent` | `bool Image.IsTransparent()` |  |
| `LoadLayout` | `bool Image.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void Image.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void Image.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void Image.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool Image.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void Image.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void Image.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void Image.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void Image.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void Image.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool Image.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void Image.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void Image.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void Image.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void Image.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void Image.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void Image.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void Image.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void Image.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void Image.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void Image.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void Image.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void Image.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void Image.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void Image.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void Image.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void Image.SetDraggable( bool  )` |  |
| `SetFocus` | `bool Image.SetFocus()` |  |
| `SetHasClass` | `void Image.SetHasClass( cstring , bool  )` |  |
| `SetImage` | `void Image.SetImage( cstring  )` |  |
| `SetInputNamespace` | `void Image.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void Image.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void Image.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void Image.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void Image.SetReadyForDisplay( bool  )` |  |
| `SetScaling` | `void Image.SetScaling( cstring  )` |  |
| `SetScrollParentToFitWhenFocused` | `void Image.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetTopOfInputContext` | `void Image.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void Image.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void Image.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void Image.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void Image.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void Image.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool Image.UpdateFocusInContext()` |  |
## Movie

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool Movie.AcceptsFocus()` |  |
| `AcceptsInput` | `bool Movie.AcceptsInput()` |  |
| `AddClass` | `void Movie.AddClass( cstring  )` |  |
| `ApplyStyles` | `void Movie.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool Movie.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool Movie.CanSeeInParentScroll()` |  |
| `Children` | `unknown Movie.Children()` |  |
| `ClearPanelEvent` | `void Movie.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void Movie.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool Movie.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown Movie.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void Movie.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void Movie.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void Movie.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown Movie.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown Movie.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown Movie.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown Movie.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 Movie.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring Movie.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 Movie.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown Movie.GetChild( int32  )` |  |
| `GetChildCount` | `int32 Movie.GetChildCount()` |  |
| `GetChildIndex` | `int32 Movie.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown Movie.GetFirstChild()` |  |
| `GetLastChild` | `unknown Movie.GetLastChild()` |  |
| `GetParent` | `unknown Movie.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown Movie.GetPositionWithinWindow()` |  |
| `HasClass` | `bool Movie.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool Movie.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool Movie.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool Movie.HasKeyFocus()` |  |
| `IsAdjustingVolume` | `bool Movie.IsAdjustingVolume()` |  |
| `IsDraggable` | `bool Movie.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool Movie.IsReadyForDisplay()` |  |
| `IsSelected` | `bool Movie.IsSelected()` |  |
| `IsTransparent` | `bool Movie.IsTransparent()` |  |
| `LoadLayout` | `bool Movie.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void Movie.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void Movie.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void Movie.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool Movie.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void Movie.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void Movie.MoveChildBefore( unknown , unknown  )` |  |
| `Pause` | `void Movie.Pause()` |  |
| `Play` | `void Movie.Play()` |  |
| `RegisterForReadyEvents` | `void Movie.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void Movie.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void Movie.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool Movie.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void Movie.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void Movie.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void Movie.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void Movie.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void Movie.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void Movie.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void Movie.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void Movie.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void Movie.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void Movie.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetControls` | `void Movie.SetControls( cstring  )` |  |
| `SetDialogVariable` | `void Movie.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void Movie.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void Movie.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void Movie.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void Movie.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void Movie.SetDraggable( bool  )` |  |
| `SetFocus` | `bool Movie.SetFocus()` |  |
| `SetHasClass` | `void Movie.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void Movie.SetInputNamespace( cstring  )` |  |
| `SetMovie` | `void Movie.SetMovie( cstring  )` |  |
| `SetPanelEvent` | `void Movie.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void Movie.SetParent( unknown  )` |  |
| `SetPlaybackVolume` | `void Movie.SetPlaybackVolume( float  )` |  |
| `SetReadyForDisplay` | `void Movie.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void Movie.SetReadyForDisplay( bool  )` |  |
| `SetRepeat` | `void Movie.SetRepeat( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void Movie.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetSound` | `void Movie.SetSound( cstring  )` |  |
| `SetTitle` | `void Movie.SetTitle( cstring  )` |  |
| `SetTopOfInputContext` | `void Movie.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void Movie.SortChildrenOnAttribute( cstring , bool  )` |  |
| `Stop` | `void Movie.Stop()` |  |
| `SwitchClass` | `void Movie.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void Movie.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void Movie.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void Movie.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool Movie.UpdateFocusInContext()` |  |
## Panel

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool Panel.AcceptsFocus()` |  |
| `AcceptsInput` | `bool Panel.AcceptsInput()` |  |
| `AddClass` | `void Panel.AddClass( cstring  )` |  |
| `ApplyStyles` | `void Panel.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool Panel.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool Panel.CanSeeInParentScroll()` |  |
| `Children` | `unknown Panel.Children()` |  |
| `ClearPanelEvent` | `void Panel.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void Panel.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool Panel.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown Panel.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void Panel.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void Panel.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void Panel.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown Panel.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown Panel.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown Panel.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown Panel.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 Panel.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring Panel.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 Panel.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown Panel.GetChild( int32  )` |  |
| `GetChildCount` | `int32 Panel.GetChildCount()` |  |
| `GetChildIndex` | `int32 Panel.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown Panel.GetFirstChild()` |  |
| `GetLastChild` | `unknown Panel.GetLastChild()` |  |
| `GetParent` | `unknown Panel.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown Panel.GetPositionWithinWindow()` |  |
| `HasClass` | `bool Panel.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool Panel.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool Panel.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool Panel.HasKeyFocus()` |  |
| `IsDraggable` | `bool Panel.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool Panel.IsReadyForDisplay()` |  |
| `IsSelected` | `bool Panel.IsSelected()` |  |
| `IsTransparent` | `bool Panel.IsTransparent()` |  |
| `LoadLayout` | `bool Panel.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void Panel.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void Panel.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void Panel.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool Panel.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void Panel.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void Panel.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void Panel.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void Panel.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void Panel.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool Panel.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void Panel.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void Panel.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void Panel.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void Panel.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void Panel.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void Panel.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void Panel.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void Panel.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void Panel.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void Panel.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void Panel.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void Panel.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void Panel.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void Panel.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void Panel.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void Panel.SetDraggable( bool  )` |  |
| `SetFocus` | `bool Panel.SetFocus()` |  |
| `SetHasClass` | `void Panel.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void Panel.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void Panel.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void Panel.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void Panel.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void Panel.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void Panel.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetTopOfInputContext` | `void Panel.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void Panel.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void Panel.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void Panel.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void Panel.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void Panel.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool Panel.UpdateFocusInContext()` |  |
## ResizeDragKnob

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'horizontalDrag' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'target' | 'unknown' | X |  |
| 'verticalDrag' | 'bool' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool ResizeDragKnob.AcceptsFocus()` |  |
| `AcceptsInput` | `bool ResizeDragKnob.AcceptsInput()` |  |
| `AddClass` | `void ResizeDragKnob.AddClass( cstring  )` |  |
| `ApplyStyles` | `void ResizeDragKnob.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool ResizeDragKnob.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool ResizeDragKnob.CanSeeInParentScroll()` |  |
| `Children` | `unknown ResizeDragKnob.Children()` |  |
| `ClearPanelEvent` | `void ResizeDragKnob.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void ResizeDragKnob.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool ResizeDragKnob.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown ResizeDragKnob.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void ResizeDragKnob.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void ResizeDragKnob.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void ResizeDragKnob.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown ResizeDragKnob.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown ResizeDragKnob.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown ResizeDragKnob.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown ResizeDragKnob.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 ResizeDragKnob.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring ResizeDragKnob.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 ResizeDragKnob.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown ResizeDragKnob.GetChild( int32  )` |  |
| `GetChildCount` | `int32 ResizeDragKnob.GetChildCount()` |  |
| `GetChildIndex` | `int32 ResizeDragKnob.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown ResizeDragKnob.GetFirstChild()` |  |
| `GetLastChild` | `unknown ResizeDragKnob.GetLastChild()` |  |
| `GetParent` | `unknown ResizeDragKnob.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown ResizeDragKnob.GetPositionWithinWindow()` |  |
| `HasClass` | `bool ResizeDragKnob.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool ResizeDragKnob.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool ResizeDragKnob.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool ResizeDragKnob.HasKeyFocus()` |  |
| `IsDraggable` | `bool ResizeDragKnob.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool ResizeDragKnob.IsReadyForDisplay()` |  |
| `IsSelected` | `bool ResizeDragKnob.IsSelected()` |  |
| `IsTransparent` | `bool ResizeDragKnob.IsTransparent()` |  |
| `LoadLayout` | `bool ResizeDragKnob.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void ResizeDragKnob.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void ResizeDragKnob.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void ResizeDragKnob.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool ResizeDragKnob.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void ResizeDragKnob.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void ResizeDragKnob.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void ResizeDragKnob.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void ResizeDragKnob.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void ResizeDragKnob.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool ResizeDragKnob.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void ResizeDragKnob.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void ResizeDragKnob.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void ResizeDragKnob.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void ResizeDragKnob.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void ResizeDragKnob.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void ResizeDragKnob.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void ResizeDragKnob.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void ResizeDragKnob.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void ResizeDragKnob.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void ResizeDragKnob.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void ResizeDragKnob.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void ResizeDragKnob.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void ResizeDragKnob.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void ResizeDragKnob.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void ResizeDragKnob.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void ResizeDragKnob.SetDraggable( bool  )` |  |
| `SetFocus` | `bool ResizeDragKnob.SetFocus()` |  |
| `SetHasClass` | `void ResizeDragKnob.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void ResizeDragKnob.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void ResizeDragKnob.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void ResizeDragKnob.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void ResizeDragKnob.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void ResizeDragKnob.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void ResizeDragKnob.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetTopOfInputContext` | `void ResizeDragKnob.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void ResizeDragKnob.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void ResizeDragKnob.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void ResizeDragKnob.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void ResizeDragKnob.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void ResizeDragKnob.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool ResizeDragKnob.UpdateFocusInContext()` |  |
## RichPresenceAPI

| Method Name | Signature | Description |
|---|---|---|
| `Clear` | `void RichPresenceAPI.Clear()` | Clears the current rich presence data |
| `UpdateRichPresenceState` | `void RichPresenceAPI.UpdateRichPresenceState( unknown key_values_object )` | Updates the current rich presence state to something new |
## StaticConsoleMessageTarget

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool StaticConsoleMessageTarget.AcceptsFocus()` |  |
| `AcceptsInput` | `bool StaticConsoleMessageTarget.AcceptsInput()` |  |
| `AddClass` | `void StaticConsoleMessageTarget.AddClass( cstring  )` |  |
| `ApplyStyles` | `void StaticConsoleMessageTarget.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool StaticConsoleMessageTarget.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool StaticConsoleMessageTarget.CanSeeInParentScroll()` |  |
| `Children` | `unknown StaticConsoleMessageTarget.Children()` |  |
| `ClearPanelEvent` | `void StaticConsoleMessageTarget.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void StaticConsoleMessageTarget.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool StaticConsoleMessageTarget.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown StaticConsoleMessageTarget.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void StaticConsoleMessageTarget.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void StaticConsoleMessageTarget.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void StaticConsoleMessageTarget.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown StaticConsoleMessageTarget.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown StaticConsoleMessageTarget.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown StaticConsoleMessageTarget.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown StaticConsoleMessageTarget.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 StaticConsoleMessageTarget.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring StaticConsoleMessageTarget.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 StaticConsoleMessageTarget.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown StaticConsoleMessageTarget.GetChild( int32  )` |  |
| `GetChildCount` | `int32 StaticConsoleMessageTarget.GetChildCount()` |  |
| `GetChildIndex` | `int32 StaticConsoleMessageTarget.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown StaticConsoleMessageTarget.GetFirstChild()` |  |
| `GetLastChild` | `unknown StaticConsoleMessageTarget.GetLastChild()` |  |
| `GetParent` | `unknown StaticConsoleMessageTarget.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown StaticConsoleMessageTarget.GetPositionWithinWindow()` |  |
| `HasClass` | `bool StaticConsoleMessageTarget.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool StaticConsoleMessageTarget.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool StaticConsoleMessageTarget.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool StaticConsoleMessageTarget.HasKeyFocus()` |  |
| `IsDraggable` | `bool StaticConsoleMessageTarget.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool StaticConsoleMessageTarget.IsReadyForDisplay()` |  |
| `IsSelected` | `bool StaticConsoleMessageTarget.IsSelected()` |  |
| `IsTransparent` | `bool StaticConsoleMessageTarget.IsTransparent()` |  |
| `LoadLayout` | `bool StaticConsoleMessageTarget.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void StaticConsoleMessageTarget.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void StaticConsoleMessageTarget.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void StaticConsoleMessageTarget.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool StaticConsoleMessageTarget.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void StaticConsoleMessageTarget.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void StaticConsoleMessageTarget.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void StaticConsoleMessageTarget.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void StaticConsoleMessageTarget.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void StaticConsoleMessageTarget.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool StaticConsoleMessageTarget.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void StaticConsoleMessageTarget.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void StaticConsoleMessageTarget.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void StaticConsoleMessageTarget.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void StaticConsoleMessageTarget.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void StaticConsoleMessageTarget.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void StaticConsoleMessageTarget.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void StaticConsoleMessageTarget.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void StaticConsoleMessageTarget.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void StaticConsoleMessageTarget.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void StaticConsoleMessageTarget.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void StaticConsoleMessageTarget.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void StaticConsoleMessageTarget.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void StaticConsoleMessageTarget.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void StaticConsoleMessageTarget.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void StaticConsoleMessageTarget.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void StaticConsoleMessageTarget.SetDraggable( bool  )` |  |
| `SetFocus` | `bool StaticConsoleMessageTarget.SetFocus()` |  |
| `SetHasClass` | `void StaticConsoleMessageTarget.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void StaticConsoleMessageTarget.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void StaticConsoleMessageTarget.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void StaticConsoleMessageTarget.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void StaticConsoleMessageTarget.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void StaticConsoleMessageTarget.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void StaticConsoleMessageTarget.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetTopOfInputContext` | `void StaticConsoleMessageTarget.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void StaticConsoleMessageTarget.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void StaticConsoleMessageTarget.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void StaticConsoleMessageTarget.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void StaticConsoleMessageTarget.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void StaticConsoleMessageTarget.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool StaticConsoleMessageTarget.UpdateFocusInContext()` |  |
## SteamOverlayAPI

| Method Name | Signature | Description |
|---|---|---|
| `OpenToProfileID` | `void SteamOverlayAPI.OpenToProfileID( cstring profileID )` | Opens the steam overlay to the given user/group profile by their steam ID. profileID is the 64bit int steam ID in a string. |
| `OpenURL` | `void SteamOverlayAPI.OpenURL( cstring url )` | Opens the steam overlay browser at the given URL |
| `OpenURLModal` | `void SteamOverlayAPI.OpenURLModal( cstring url )` | Opens the steam overlay browser at the given URL in a modal window (no other windows in overlay, and overlay closes when window closes) |
## ToggleButton

| Property Name | Type | ReadOnly | Description |
|---|---|---|---|
| 'activationenabled' | 'bool' |   |  |
| 'actuallayoutheight' | 'float' | X |  |
| 'actuallayoutwidth' | 'float' | X |  |
| 'actualuiscale_x' | 'float' | X |  |
| 'actualuiscale_y' | 'float' | X |  |
| 'actualxoffset' | 'float' | X |  |
| 'actualyoffset' | 'float' | X |  |
| 'checked' | 'bool' |   |  |
| 'contentheight' | 'float' | X |  |
| 'contentwidth' | 'float' | X |  |
| 'defaultfocus' | 'cstring' |   |  |
| 'desiredlayoutheight' | 'float' | X |  |
| 'desiredlayoutwidth' | 'float' | X |  |
| 'enabled' | 'bool' |   |  |
| 'hittest' | 'bool' |   |  |
| 'hittestchildren' | 'bool' |   |  |
| 'id' | 'cstring' | X |  |
| 'inputnamespace' | 'cstring' |   |  |
| 'layoutfile' | 'cstring' | X |  |
| 'paneltype' | 'cstring' | X |  |
| 'rememberchildfocus' | 'bool' |   |  |
| 'scrolloffset_x' | 'float' | X |  |
| 'scrolloffset_y' | 'float' | X |  |
| 'selectionpos_x' | 'float' |   |  |
| 'selectionpos_y' | 'float' |   |  |
| 'style' | 'unknown' | X |  |
| 'tabindex' | 'float' |   |  |
| 'text' | 'cstring' |   |  |
| 'visible' | 'bool' |   |  |

| Method Name | Signature | Description |
|---|---|---|
| `AcceptsFocus` | `bool ToggleButton.AcceptsFocus()` |  |
| `AcceptsInput` | `bool ToggleButton.AcceptsInput()` |  |
| `AddClass` | `void ToggleButton.AddClass( cstring  )` |  |
| `ApplyStyles` | `void ToggleButton.ApplyStyles( bool  )` |  |
| `BAscendantHasClass` | `bool ToggleButton.BAscendantHasClass( cstring  )` |  |
| `CanSeeInParentScroll` | `bool ToggleButton.CanSeeInParentScroll()` |  |
| `Children` | `unknown ToggleButton.Children()` |  |
| `ClearPanelEvent` | `void ToggleButton.ClearPanelEvent( cstring  )` |  |
| `ClearPropertyFromCode` | `void ToggleButton.ClearPropertyFromCode( unknown  )` |  |
| `CreateChildren` | `bool ToggleButton.CreateChildren( cstring  )` |  |
| `CreateCopyOfCSSKeyframes` | `unknown ToggleButton.CreateCopyOfCSSKeyframes( cstring  )` |  |
| `Data` | `void ToggleButton.Data( js_raw_arg  )` |  |
| `DeleteAsync` | `void ToggleButton.DeleteAsync( float  )` |  |
| `DeleteKeyframes` | `void ToggleButton.DeleteKeyframes( unknown  )` |  |
| `FindChild` | `unknown ToggleButton.FindChild( cstring  )` |  |
| `FindChildInLayoutFile` | `unknown ToggleButton.FindChildInLayoutFile( cstring  )` |  |
| `FindChildrenWithClassTraverse` | `unknown ToggleButton.FindChildrenWithClassTraverse( cstring  )` |  |
| `FindChildTraverse` | `unknown ToggleButton.FindChildTraverse( cstring  )` |  |
| `GetAttributeInt` | `int32 ToggleButton.GetAttributeInt( cstring , int32  )` |  |
| `GetAttributeString` | `cstring ToggleButton.GetAttributeString( cstring , cstring  )` |  |
| `GetAttributeUInt32` | `uint32 ToggleButton.GetAttributeUInt32( cstring , uint32  )` |  |
| `GetChild` | `unknown ToggleButton.GetChild( int32  )` |  |
| `GetChildCount` | `int32 ToggleButton.GetChildCount()` |  |
| `GetChildIndex` | `int32 ToggleButton.GetChildIndex( unknown  )` |  |
| `GetFirstChild` | `unknown ToggleButton.GetFirstChild()` |  |
| `GetLastChild` | `unknown ToggleButton.GetLastChild()` |  |
| `GetParent` | `unknown ToggleButton.GetParent()` |  |
| `GetPositionWithinWindow` | `unknown ToggleButton.GetPositionWithinWindow()` |  |
| `HasClass` | `bool ToggleButton.HasClass( cstring  )` |  |
| `HasDescendantKeyFocus` | `bool ToggleButton.HasDescendantKeyFocus()` |  |
| `HasHoverStyle` | `bool ToggleButton.HasHoverStyle()` |  |
| `HasKeyFocus` | `bool ToggleButton.HasKeyFocus()` |  |
| `IsDraggable` | `bool ToggleButton.IsDraggable()` |  |
| `IsReadyForDisplay` | `bool ToggleButton.IsReadyForDisplay()` |  |
| `IsSelected` | `bool ToggleButton.IsSelected()` |  |
| `IsTransparent` | `bool ToggleButton.IsTransparent()` |  |
| `LoadLayout` | `bool ToggleButton.LoadLayout( cstring , bool , bool  )` |  |
| `LoadLayoutAsync` | `void ToggleButton.LoadLayoutAsync( cstring , bool , bool  )` |  |
| `LoadLayoutFromString` | `void ToggleButton.LoadLayoutFromString( js_raw_arg  )` |  |
| `LoadLayoutFromStringAsync` | `void ToggleButton.LoadLayoutFromStringAsync( cstring , bool , bool  )` |  |
| `LoadLayoutSnippet` | `bool ToggleButton.LoadLayoutSnippet( cstring  )` |  |
| `MoveChildAfter` | `void ToggleButton.MoveChildAfter( unknown , unknown  )` |  |
| `MoveChildBefore` | `void ToggleButton.MoveChildBefore( unknown , unknown  )` |  |
| `RegisterForReadyEvents` | `void ToggleButton.RegisterForReadyEvents( bool  )` |  |
| `RemoveAndDeleteChildren` | `void ToggleButton.RemoveAndDeleteChildren()` |  |
| `RemoveClass` | `void ToggleButton.RemoveClass( cstring  )` |  |
| `ScrollParentToFitWhenFocused` | `bool ToggleButton.ScrollParentToFitWhenFocused()` |  |
| `ScrollParentToMakePanelFit` | `void ToggleButton.ScrollParentToMakePanelFit( unknown , bool  )` |  |
| `ScrollToBottom` | `void ToggleButton.ScrollToBottom()` |  |
| `ScrollToFitRegion` | `void ToggleButton.ScrollToFitRegion( float , float , float , float , unknown , bool , bool  )` |  |
| `ScrollToLeftEdge` | `void ToggleButton.ScrollToLeftEdge()` |  |
| `ScrollToRightEdge` | `void ToggleButton.ScrollToRightEdge()` |  |
| `ScrollToTop` | `void ToggleButton.ScrollToTop()` |  |
| `SetAcceptsFocus` | `void ToggleButton.SetAcceptsFocus( bool  )` |  |
| `SetAttributeInt` | `void ToggleButton.SetAttributeInt( cstring , int32  )` |  |
| `SetAttributeString` | `void ToggleButton.SetAttributeString( cstring , cstring  )` |  |
| `SetAttributeUInt32` | `void ToggleButton.SetAttributeUInt32( cstring , uint32  )` |  |
| `SetDialogVariable` | `void ToggleButton.SetDialogVariable( cstring , cstring  )` |  |
| `SetDialogVariableFloat` | `void ToggleButton.SetDialogVariableFloat( cstring , float  )` |  |
| `SetDialogVariableInt` | `void ToggleButton.SetDialogVariableInt( cstring , int32  )` |  |
| `SetDialogVariableTime` | `void ToggleButton.SetDialogVariableTime( cstring , unknown  )` |  |
| `SetDisableFocusOnMouseDown` | `void ToggleButton.SetDisableFocusOnMouseDown( bool  )` |  |
| `SetDraggable` | `void ToggleButton.SetDraggable( bool  )` |  |
| `SetFocus` | `bool ToggleButton.SetFocus()` |  |
| `SetHasClass` | `void ToggleButton.SetHasClass( cstring , bool  )` |  |
| `SetInputNamespace` | `void ToggleButton.SetInputNamespace( cstring  )` |  |
| `SetPanelEvent` | `void ToggleButton.SetPanelEvent( js_raw_arg  )` |  |
| `SetParent` | `void ToggleButton.SetParent( unknown  )` |  |
| `SetReadyForDisplay` | `void ToggleButton.SetReadyForDisplay( bool  )` |  |
| `SetReadyForDisplay` | `void ToggleButton.SetReadyForDisplay( bool  )` |  |
| `SetScrollParentToFitWhenFocused` | `void ToggleButton.SetScrollParentToFitWhenFocused( bool  )` |  |
| `SetSelected` | `void ToggleButton.SetSelected( bool  )` |  |
| `SetTopOfInputContext` | `void ToggleButton.SetTopOfInputContext( bool  )` |  |
| `SortChildrenOnAttribute` | `void ToggleButton.SortChildrenOnAttribute( cstring , bool  )` |  |
| `SwitchClass` | `void ToggleButton.SwitchClass( cstring , cstring  )` |  |
| `ToggleClass` | `void ToggleButton.ToggleClass( cstring  )` |  |
| `TriggerClass` | `void ToggleButton.TriggerClass( cstring  )` |  |
| `UpdateCurrentAnimationKeyframes` | `void ToggleButton.UpdateCurrentAnimationKeyframes( unknown  )` |  |
| `UpdateFocusInContext` | `bool ToggleButton.UpdateFocusInContext()` |  |
## UiToolkitAPI
Helper to show popups, tooltips, context menus and to register/invoke js callbacks.

| Method Name | Signature | Description |
|---|---|---|
| `AddDenyAllInputToGame` | `uint64 UiToolkitAPI.AddDenyAllInputToGame( unknown panelPtr, cstring strDebugContextName )` | Denies input to the game by filtering input events. Returns a handle used by ReleaseDenyAllInputToGame. |
| `AddDenyMouseInputToGame` | `uint64 UiToolkitAPI.AddDenyMouseInputToGame( unknown panelPtr, cstring strDebugContextName )` | Denies mouse input to the game by filtering mouse input events. Returns a handle used by ReleaseDenyMouseInputToGame. |
| `CloseAllVisiblePopups` | `void UiToolkitAPI.CloseAllVisiblePopups()` | Force closing all visible popups |
| `GetGlobalObject` | `void UiToolkitAPI.GetGlobalObject( js_raw_arg  )` | Returns a global object that can be used to store global variables you would like to share across js files. |
| `HideCustomLayoutTooltip` | `void UiToolkitAPI.HideCustomLayoutTooltip( cstring tooltipID )` | Hide the tooltip with the given id. |
| `HideTextTooltip` | `void UiToolkitAPI.HideTextTooltip()` | Hide the text tooltip |
| `HideTitleImageTextTooltip` | `void UiToolkitAPI.HideTitleImageTextTooltip()` | Hide the title image text tooltip |
| `HideTitleTextTooltip` | `void UiToolkitAPI.HideTitleTextTooltip()` | Hide the title text tooltip |
| `InvokeJSCallback` | `void UiToolkitAPI.InvokeJSCallback( js_raw_arg  )` | Invoke a javascript callback using a handle previously registered with RegisterJSCallback. First argument must be the callback handle followed by the callback's arguments. |
| `IsPanoramaInECOMode` | `bool UiToolkitAPI.IsPanoramaInECOMode()` | Is Panorama in ECO (perf) mode |
| `MakeStringSafe` | `cstring UiToolkitAPI.MakeStringSafe( cstring str )` |  |
| `ProfilingScopeBegin` | `void UiToolkitAPI.ProfilingScopeBegin( cstring tagName )` | Notify telemetry that a zone is been entered |
| `ProfilingScopeEnd` | `double UiToolkitAPI.ProfilingScopeEnd()` | Notify telemetry that a zone is been left. Returns duration in milliseconds. |
| `RegisterHUDPanel2d` | `void UiToolkitAPI.RegisterHUDPanel2d( cstring panelTypeName, cstring layoutFile )` | Register a HUD panel type name with the corresponding layout file |
| `RegisterJSCallback` | `int32 UiToolkitAPI.RegisterJSCallback( unknown jsCallbackFunc )` | Register a javascript callback that can be invoke at a later stage using InvokeJSCallback. Returns a callback handle. |
| `RegisterPanel2d` | `void UiToolkitAPI.RegisterPanel2d( cstring panelTypeName, cstring layoutFile )` | Register a panel type name with the corresponding layout file |
| `ReleaseDenyAllInputToGame` | `void UiToolkitAPI.ReleaseDenyAllInputToGame( uint64 handle )` | ReleaseDenyAllInputToGame takes a handle as parameters previously returned by AddDenyAllInputToGame |
| `ReleaseDenyMouseInputToGame` | `void UiToolkitAPI.ReleaseDenyMouseInputToGame( uint64 handle )` | ReleaseDenyMouseInputToGame takes a handle as parameters previously returned by AddDenyMouseInputToGame |
| `ShowCustomLayoutContextMenu` | `unknown UiToolkitAPI.ShowCustomLayoutContextMenu( cstring targetPanelID, cstring contentmenuID, cstring layoutFile )` | Show a context menu with a specific id and using the given layout. targetPanelID  can be the empty string in which case the cursor position is used to position the context menu. Returns context menu panel. |
| `ShowCustomLayoutContextMenuParameters` | `unknown UiToolkitAPI.ShowCustomLayoutContextMenuParameters( cstring targetPanelID, cstring contentmenuID, cstring layoutFile, cstring parameters )` | Show a context menu with a specific id and using the given layout and parameters. targetPanelID  can be the empty string in which case the cursor position is used to position the context menu. Returns context menu panel. |
| `ShowCustomLayoutContextMenuParametersDismissEvent` | `unknown UiToolkitAPI.ShowCustomLayoutContextMenuParametersDismissEvent( cstring targetPanelID, cstring contentmenuID, cstring layoutFile, cstring parameters, unknown dismissJsFunc )` | Show a context menu with a specific id and using the given layout and parameters and call a function when dismissed. targetPanelID  can be the empty string in which case the cursor position is used to position the context menu. Returns context menu panel. |
| `ShowCustomLayoutParametersTooltip` | `void UiToolkitAPI.ShowCustomLayoutParametersTooltip( cstring targetPanelID, cstring tooltipID, cstring layoutFile, cstring parameters )` | Show a tooltip with a specifix id and using the given layout and parameters. |
| `ShowCustomLayoutParametersTooltipStyled` | `void UiToolkitAPI.ShowCustomLayoutParametersTooltipStyled( cstring targetPanelID, cstring tooltipID, cstring layoutFile, cstring parameters, cstring style )` | Show a tooltip with a specifix id and using the given layout and parameters. Also apply a CSS class named "style" (to the tooltip root panel) in order to allow custom styling (eg. "Tooltip_NoArrow" to remove tooltip's arrow). |
| `ShowCustomLayoutPopup` | `unknown UiToolkitAPI.ShowCustomLayoutPopup( cstring popupID, cstring layoutFile )` | Show a popup that lets you specify a layout. |
| `ShowCustomLayoutPopupParameters` | `unknown UiToolkitAPI.ShowCustomLayoutPopupParameters( cstring popupID, cstring layoutFile, cstring parameters )` | Show a popup that lets you specify a layout and parameters. |
| `ShowCustomLayoutTooltip` | `void UiToolkitAPI.ShowCustomLayoutTooltip( cstring targetPanelID, cstring tooltipID, cstring layoutFile )` | Show a tooltip with a specifix id and using the given layout. |
| `ShowCustomLayoutTooltipStyled` | `void UiToolkitAPI.ShowCustomLayoutTooltipStyled( cstring targetPanelID, cstring tooltipID, cstring layoutFile, cstring style )` | Show a tooltip with a specifix id and using the given layout. Also apply a CSS class named "style" (to the tooltip root panel) in order to allow custom styling (eg. "Tooltip_NoArrow" to remove tooltip's arrow). |
| `ShowGenericPopup` | `unknown UiToolkitAPI.ShowGenericPopup( cstring title, cstring message, cstring style )` | Show a popup with the given title add message and optional style. Button present: "OK". |
| `ShowGenericPopupBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupBgStyle( cstring title, cstring message, cstring style, cstring bgStyle )` | Show a popup with the given title add message and optional style. You can specify the background style ("none", "dim" or "blur"). Button present: "OK". |
| `ShowGenericPopupCancel` | `unknown UiToolkitAPI.ShowGenericPopupCancel( cstring title, cstring message, cstring style, unknown cancelJSFunc )` | Show a popup with the given title add message and optional style. Button present: "Cancel". |
| `ShowGenericPopupCancelBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupCancelBgStyle( cstring title, cstring message, cstring style, unknown cancelJSFunc, cstring bgStyle )` | Show a popup with the given title add message and optional style. You can specify the background style ("none", "dim" or "blur"). Button present: "Cancel". |
| `ShowGenericPopupOk` | `unknown UiToolkitAPI.ShowGenericPopupOk( cstring title, cstring message, cstring style, unknown okJSFunc )` | Show a popup with the given title add message and optional style. Button present: "OK". |
| `ShowGenericPopupOkBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupOkBgStyle( cstring title, cstring message, cstring style, unknown okJSFunc, cstring bgStyle )` | Show a popup with the given title add message and optional style. You can specify the background style ("none", "dim" or "blur"). Button present: "OK". |
| `ShowGenericPopupOkCancel` | `unknown UiToolkitAPI.ShowGenericPopupOkCancel( cstring title, cstring message, cstring style, unknown okJSFunc, unknown cancelJSFunc )` | Show a popup with the given title add message and optional style. Button present: "Ok"/"Cancel". |
| `ShowGenericPopupOkCancelBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupOkCancelBgStyle( cstring title, cstring message, cstring style, unknown okJSFunc, unknown cancelJSFunc, cstring bgStyle )` | Show a popup with the given title add message and optional style. You can specify the background style ("none", "dim" or "blur"). Button present: "Ok"/"Cancel". |
| `ShowGenericPopupOneOption` | `unknown UiToolkitAPI.ShowGenericPopupOneOption( cstring title, cstring message, cstring style, cstring optionName, unknown optionJSFunc )` | Show a popup with the given title add message and optional style and let you specify the name of one button. |
| `ShowGenericPopupOneOptionBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupOneOptionBgStyle( cstring title, cstring message, cstring style, cstring optionName, unknown optionJSFunc, cstring bgStyle )` | Show a popup with the given title add message and optional style and let you specify the name of one button. You can specify the background style ("none", "dim" or "blur").  |
| `ShowGenericPopupThreeOptions` | `unknown UiToolkitAPI.ShowGenericPopupThreeOptions( cstring title, cstring message, cstring style, cstring option1Name, unknown option1JSFunc, cstring option2Name, unknown option2JSFunc, cstring option3Name, unknown option3JSFunc )` | Show a popup with the given title add message and optional style and let you specify the name of two button. |
| `ShowGenericPopupThreeOptionsBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupThreeOptionsBgStyle( cstring title, cstring message, cstring style, cstring option1Name, unknown option1JSFunc, cstring option2Name, unknown option2JSFunc, cstring option3Name, unknown option3JSFunc, cstring bgStyle )` | Show a popup with the given title add message and optional style and let you specify the name of two button. You can specify the background style ("none", "dim" or "blur").  |
| `ShowGenericPopupTwoOptions` | `unknown UiToolkitAPI.ShowGenericPopupTwoOptions( cstring title, cstring message, cstring style, cstring option1Name, unknown option1JSFunc, cstring option2Name, unknown option2JSFunc )` | Show a popup with the given title add message and optional style and let you specify the name of two button. |
| `ShowGenericPopupTwoOptionsBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupTwoOptionsBgStyle( cstring title, cstring message, cstring style, cstring option1Name, unknown option1JSFunc, cstring option2Name, unknown option2JSFunc, cstring bgStyle )` | Show a popup with the given title add message and optional style and let you specify the name of two button. You can specify the background style ("none", "dim" or "blur").  |
| `ShowGenericPopupYesNo` | `unknown UiToolkitAPI.ShowGenericPopupYesNo( cstring title, cstring message, cstring style, unknown yesJSFunc, unknown noJSFunc )` | Show a popup with the given title add message and optional style. Button present: "Yes"/"No". |
| `ShowGenericPopupYesNoBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupYesNoBgStyle( cstring title, cstring message, cstring style, unknown yesJSFunc, unknown noJSFunc, cstring bgStyle )` | Show a popup with the given title add message and optional style. You can specify the background style ("none", "dim" or "blur"). Button present: "Yes"/"No". |
| `ShowGenericPopupYesNoCancel` | `unknown UiToolkitAPI.ShowGenericPopupYesNoCancel( cstring title, cstring message, cstring style, unknown yesJSFunc, unknown noJSFunc, unknown cancelJSFunc )` | Show a popup with the given title add message and optional style. Button present: "Yes"/"No"/"Cancel". |
| `ShowGenericPopupYesNoCancelBgStyle` | `unknown UiToolkitAPI.ShowGenericPopupYesNoCancelBgStyle( cstring title, cstring message, cstring style, unknown yesJSFunc, unknown noJSFunc, unknown cancelJSFunc, cstring bgStyle )` | Show a popup with the given title add message and optional style. You can specify the background style ("none", "dim" or "blur"). Button present: "Yes"/"No"/"Cancel". |
| `ShowGlobalCustomLayoutPopup` | `unknown UiToolkitAPI.ShowGlobalCustomLayoutPopup( cstring popupID, cstring layoutFile )` | Show a popup on the 'global popups top level window' that lets you specify a layout. |
| `ShowGlobalCustomLayoutPopupParameters` | `unknown UiToolkitAPI.ShowGlobalCustomLayoutPopupParameters( cstring popupID, cstring layoutFile, cstring parameters )` | Show a popup on 'global popups top level window' that lets you specify a layout and parameters. |
| `ShowSimpleContextMenu` | `unknown UiToolkitAPI.ShowSimpleContextMenu( cstring targetPanelID, cstring contentmenuID, unknown items )` | Show a context menu with a specific id and populate the context menu item list using the given "items" array. Each elements of the items array is a javascript object of the form {label, jsCallback, style, icon}. targetPanelID  can be the empty string in which case the cursor position is used to position the context menu. Returns context menu panel. |
| `ShowSimpleContextMenuWithDismissEvent` | `unknown UiToolkitAPI.ShowSimpleContextMenuWithDismissEvent( cstring targetPanelID, cstring contentmenuID, unknown items, unknown dismissJsFunc )` | Show a context menu with a specific id and populate the context menu item list using the given "items" array. Each elements of the items array is a javascript object of the form {label, jsCallback, style, icon}. targetPanelID  can be the empty string in which case the cursor position is used to position the context menu. Returns context menu panel. |
| `ShowTextTooltip` | `void UiToolkitAPI.ShowTextTooltip( cstring targetPanelID, cstring text )` | Show a tooltip with the given text |
| `ShowTextTooltipOnPanel` | `void UiToolkitAPI.ShowTextTooltipOnPanel( unknown targetPanel, cstring text )` | Show a tooltip with the given text on given panel |
| `ShowTextTooltipOnPanelStyled` | `void UiToolkitAPI.ShowTextTooltipOnPanelStyled( unknown targetPanel, cstring text, cstring style )` | Show a tooltip with the given text on given panel. Also apply a CSS class named "style" to allow custom styling. |
| `ShowTextTooltipStyled` | `void UiToolkitAPI.ShowTextTooltipStyled( cstring targetPanelID, cstring text, cstring style )` | Show a tooltip with the given text. Also apply a CSS class named "style" to allow custom styling. |
| `ShowTitleImageTextTooltip` | `void UiToolkitAPI.ShowTitleImageTextTooltip( cstring targetPanelID, cstring title, cstring image, cstring text )` | Show a tooltip with the given title, image and text. |
| `ShowTitleImageTextTooltipStyled` | `void UiToolkitAPI.ShowTitleImageTextTooltipStyled( cstring targetPanelID, cstring title, cstring image, cstring text, cstring style )` | Show a tooltip with the giben title, image and text. Also apply a CSS class named "style" to allow custom styling. |
| `ShowTitleTextTooltip` | `void UiToolkitAPI.ShowTitleTextTooltip( cstring targetPanelID, cstring title, cstring text )` | Show a tooltip with the given title and text. |
| `ShowTitleTextTooltipStyled` | `void UiToolkitAPI.ShowTitleTextTooltipStyled( cstring targetPanelID, cstring title, cstring text, cstring style )` | Show a tooltip with the given title and text. Also apply a CSS class named "style" to allow custom styling. |
| `UnregisterJSCallback` | `void UiToolkitAPI.UnregisterJSCallback( int32 jsCallbackHandle )` | Unregister a javascript callback previously registered with RegisterJSCallback. |
## UserAPI

| Method Name | Signature | Description |
|---|---|---|
| `GetXUID` | `uint64 UserAPI.GetXUID()` | Gets the XUID (steamid as integer) of the local player |