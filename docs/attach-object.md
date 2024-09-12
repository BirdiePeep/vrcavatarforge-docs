# Attach Object



Allows objects to attach themselves onto the avatar.  This feature will also re-attach bones from matching SkinnedMeshRenderers, enabling clothing to move with the avatar.

- **Source:** The object you want to move onto the avatar.  If no Source is provided it will use the object this Feature is attached to.
- **Attach Target:**
	- **Root:** Attaches to the root of the avatar.
	- **Path:** Attaches to a string path provided assuming it can be found on the avatar.
	- **Humanoid Bone:** Attaches to a specific humanoid bone, this is generic across all humanoid avatars.
- **Merge Transforms:** When enabled, any objects with the same path as existing objects on the avatar will not be moved.  This is useful when attaching an object with a similar armature as you only want one set of bones.
- **Keep World Position:** When enabled, objects moved will keep their current world position.  Sometimes this is useful if an attachment is not specifically setup for the target avatar.
- **Attach Children Instead:** When enabled, instead of attaching the Source all of the source's children will be moved to the target.

> [!NOTE]
> Objects using this feature need to be placed somewhere on the avatar for the attachment to work.  The exact location doesn't matter, but typically users will drag these onto the root of the avatar.  For Example...
>
> ![attach-object](~/images/attach-object-attach.png)



> [!NOTE]
> When an object is attached we attempt to match any new SkinnedMeshRenderer bones with existing transforms.  Bone references will be looked up at it's new location and replaced with that new bone reference.  This only works if the bones from the source and target share an armature with the exact same path names.  Any bones without a matching transform at the new location will be left as their original value.

