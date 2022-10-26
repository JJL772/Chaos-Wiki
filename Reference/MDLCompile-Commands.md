---
title: MDLCompile/StudioMDL Commands
description: List of all studiomdl commands
published: true
date: 2022-10-26T07:09:19.351Z
tags: engine, reference
editor: markdown
dateCreated: 2022-10-26T07:09:19.351Z
---

# List of StudioMDL/MDLCompile commands (.qc or .mc scripts)

| Command | Parameters | Description |
|---|---|---|
| `$cd` | `string directory` | Directory to change to |
| `$modelname` | `string modelName` | Set the name of the model, relative to the `models/` directory, including the `.mdl` extension |
| `$internalname` | `string internalName` | Set the internal name of the model. This will be used as the name of the `.ani` file |
| `$cdmaterials` | `string materialsPath` | Set the materials path |
| `$pushd` | `string directory` | Same as `$cd` but pushes the current directory to a stack before doing the cd |
| `$popd` | none | Return to the directory previous to the last `$pushd` call |
| `$scale` | `float flScale` | Scale the model on all axes by a scalar value |
| `$root` | `string boneName` | Set the name of the root bone |
| `$controller` | | |
| `$screenalign` | `string boneName, string type = ["sphere", "cylinder", "billboard"]` | Align bone with screen |
| `$worldalign` | `string boneName` | Align bone with world |
| `$keepupright` | `string boneName` | Keeps a bone upright |
| `$model` | | |
| `$collisionmodel` | `string modelName, [optional block]` | Set the collision model for the mesh |
| `$collisionjoints` | `string modelName, [optional block]` | Set the collision model for the mesh, with separate joints |
| `$collisiontext` | | |
| `$appendsource` | | |
| `$body` | | |
| `$prefer_fbx` | | |
| `$bodygroup` | | |
| `$appendblankbodygroup` | | |
| `$bodygrouppreset` | | |
| `$animation` | | |
| `$autocenter` | | |
| `$sequence` | | |
| `$append` | | |
| `$prepend` | | |
| `$continue` | | |
| `$declaresequence` | | |
| `$declareanimation` | | |
| `$cmdlist` | | |
| `$animblocksize` | | |
| `$weightlist` | | |
| `$defaultweightlist` | | |
| `$ikchain` | | |
| `$ikautoplaylock` | | |
| `$eyeposition` | | |
| `$illumposition` | | |
| `$origin` | | |
| `$originbones` | | |
| `$upaxis` | | |
| `$bbox` | | |
| `$bboxonlyverts` | | |
| `$cbox` | | |
| `$gamma` | | |
| `$texturegroup` | | |
| `$hgroup` | | |
| `$hbox` | | |
| `$hboxset` | | |
| `$surfaceprop` | | |
| `$jointsurfaceprop` | | |
| `$contents` | `string contents = ["grate", "ladder", "solid", "monster", "notsolid"]` | |
| `$jointcontents` | `string jointName, string contents = ["grate", "ladder", "solid", "monster", "notsolid"]` | |
| `$attachment` | | |
| `$redefineattachment` | | |
| `$bonemerge` | | |
| `$bonealwayssetup` | | |
| `$externaltextures` | | |
| `$cliptotextures` | | |
| `$skinnedLODs` | | |
| `$renamebone` | | |
| `$stripboneprefix` | | |
| `$renamebonesubstr` | | |
| `$collapsebones` | | |
| `$collapsebonesaggressive` | | |
| `$alwayscollapse` | | |
| `$proceduralbones` | | |
| `$skiptransition` | | |
| `$calctransitions` | | |
| `$staticprop` | none | Mark this model as a static prop |
| `$zbrush` | none | Enable some special processing for zbrush authored models. Models marked with this have their texcoords smoothed. This is very expensive! |
| `$realignbones` | | |
| `$forcerealign` | | |
| `$lod` | | |
| `$shadowlod` | | |
| `$poseparameter` | | |
| `$heirarchy` | | Lol, lmao|
| `$hierarchy` | | |
| `$insertbone` | | |
| `$limitrotation` | | |
| `$definebone` | | |
| `$jigglebone` | | |
| `$includemodel` | | |
| `$opaque` | none | Force this model to be opaque. Removes any transparency flags |
| `$mostlyopaque` | | |
| `$keyvalues` | `block` | Defines a block of key-value pairs. These will be embedded into the model |
| `$obsolete` | none | Marks this model as obsolete. It will show the obsolete material in-game |
| `$renamematerial` | | |
| `$renamematerialsubstr` | | |
| `$overridematerial` | | |
| `$stripmaterialpaths` | | |
| `$fakevta` | | |
| `$noforcedfade` | | |
| `$skipboneinbbox` | | |
| `$forcephonemecrossfade` | | |
| `$lockbonelengths` | | |
| `$unlockdefinebones` | | |
| `$constantdirectionallight` | `float flDirLightDot` | Set the constant directional light dot product. Must be between 0 and 1, floating point number |
| `$minlod` | `int minLod` | Set the min lod |
| `$allowrootlods` | | |
| `$bonesaveframe` | | |
| `$ambientboost` | none | Indicate that the model should be rendered with an ambient boost |
| `$centerbonesonverts` | | |
| `$donotcastshadows` | none | Indicate that the model should not cast any shadows |
| `$casttextureshadows` | none | Indicate that this model should cast texture-based shadows in vrad, only applies to prop_static |
| `$motionrollback` | | |
| `$sectionframes` | | |
| `$clampworldspace` | | |
| `$maxeyedeflection` | | |
| `$addsearchdir` | | |
| `$phyname` | | |
| `$subd` | none | Indicate that we have a quad-only catmull-clark subd mesh in the model |
| `$boneflexdriver` | | |
| `$maxverts` | `int maxVerts` | Set the max verts on the model. Must be in range [1024, 65536] |
| `$preservetriangleorder` | | |
| `$qcassert` | | |
| `$lcaseallsequences` | | |
| `$defaultfadein` | | |
| `$defaultfadeout` | | |
| `$cloth` | | |
| `$clothplanecollision` | | |
| `$allowactivityname` | | |
| `$collisionprecision` | | |
| `$erroronsequenceremappingfailure` | | |
| `$erroronsequenceremappingfailure_disable` | | |
| `$modelhasnosequences` | | |
| `$contentrootrelative` | | |
| `$adduvmapchannelto` | | |
| `$section` | | |
| `$sectionenable` | | |
| `$sectiondisable` | | |