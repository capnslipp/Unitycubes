# Unitycubes

Unitycubes is a package manager for Unity3D game libraries that is founded on a few principles:

1. **The official Unity Asset Store sucks for libraries**  
   The Asset Store is filled to the brim with seemingly useful libraries— at $10-100 a pop.  Some are worth the cost, most aren't.  And since library devs want to justify the cost of their add-ons, simple scripts are a rarity in favor of large toolkits.  Most of these large libraries are built on custom object models and are incompatible with each other.
2. **The UnityCommunity wiki and forums were great/sucked for libraries**  
   The Unity forums and the UnityCommunity wiki were great resources to find useful libraries and learn Unity coding by-example early on.  The [wiki's scripts section](http://wiki.unity3d.com/index.php/Scripts "Unify Community Wiki - Scripts") was at a time the central shared repo of Unity library code.  However, this fell to the wayside as multiple versions of scripts popped up, as Unity deprecated old API calls breaking scripts, as the Unity Answers Q&A site took over the role of one-off programming questions, and as the allure of profit via the official Asset Store took over.
3. **Current Unity libaries are dev-heavy**  
   In an effort to overcome incompatiblities with others' libs and distinquish one's own code, Unity library devs have resorted to distributing their code as large kitchen-sink libraries, heavily prefixed with thier own name.  This self-centered approach inhibits the community from improving and building on each other's libraries.
4. **.unitypackages don't do the job.**  
   While the built-in `.unitypackage` format is well-suited for serializing assets together in a way reconstrutable in another Unity project, libraries have little-to-no non-code assets, and really shouldn't rely on editor associations.   `.unitypackage` also don't provide any mechanism for stating dependencies on other libaries or Unity engine versions.
5. **Ruby has Gems, Python has Eggs…**  
   While Unity could probably use something like [NuGet](http://www.nuget.org/), Unity is more of an independent environment just utilizing C#, Boo, and [UnityScript](https://github.com/bamboo/unityscript), with its own filesystem structure, build system, and other concerns.


## Development Status / Usage

Unitycubes is currently a work-in-progress prototype.

For now, pulling individual `Library/…` subdirs into your project should work just as well as grabbing Unity code from anywhere else.  Pull requests for Library additions here on GitHub will be considered.
