# Efficient Workflows
---
## Multi Scene Workflow

Each chunk of the app is divided into multiple scene, and the scenes are loaded during runtime.

![[Pasted image 20210914191607.png]]

### Pros

##### Makes collaboration easier
Different developers can segment each scene into different scenes are then work on them separately. Afterwards, we  either merge them together OR load them during runtime.

### Cons

##### 1. Cross scene referencing is not allowed in unity 

That is if a game object from one scene references a game object from another. If the scenes are both active, they will work fine, but as soon as any one of them unloads, the reference will be lost, resulting in errors. 

##### 2. Lag spikes

Scene loading during runtime introduces lag spikes if a lot of objects are activated at once. More issues with physical rigid bodies.

### Work around

##### 1. Custom solution

We are either write custom scripts that handle scene loading in such a way that prevents all the game objects being loaded at the same time.



##### 2.Merging

We can simple merge the scene after the developers have done working on them. There shouldn't be any issues with merging because each scene contains unique items.

---

## Using Prefabs

Treating each small component as a separate prefab.

Every time a developer wants to add something new to a scene, they create a unity prefab.

![[Pasted image 20210914192651.png]]

Then they do all their work inside the prefab editor instead of the scene editor.

![[Pasted image 20210914192814.png]]

### Pros
Gets rid of issues of scene merging all together. The developer is no longer working in a scene, instead they are working in a prefab that will be packaged separately.

### Cons
[TODO]