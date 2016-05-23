Alas, it's not possible to keep compatibility with any single mod in the KSP world. Sometimes, third-party mods modify game so what KIS cannot work properly. Or, vise-versa, KIS modifications make other mods to fail. The list below is **not** a "shame list", it's just a way to reduce support efforts.

If you've noticed another mod that conflicts with KIS, please, notify on the [forum's thread](http://forum.kerbalspaceprogram.com/index.php?/topic/101928-110-kerbal-inventory-system-kis-127/). If you've noticed one of the mods in the list is no more conflicting with KIS, please, also notify on the forum's thread.

### List of incompatible mods

- *Infernal robotics*. KIS is unable to correctly attach/detach IR parts due to their complexity. There is no ETA to fix it.
- *Kerbal Krash System*. Will cause kerbal replication issue on every new KIS release due to failed dependency. It's not KKS or KIS bug, it's an issue of the game engine (see [issue](http://bugs.kerbalspaceprogram.com/issues/9752) on bugtracker). The workround for now is downgrading KIS or disabling KKS until the latter is re-compiled with the latest KIS version. There is no ETA to fix this problem.
- *Deadly Reentry*. As of v7.4.2 is known to cause kerbal replication bug when entering a pod. This is not a KIS issue.
- *Kerbalism*. As of v0.9.9.4 is known to cause kerbal replication bug when entering a pod. This is not a KIS issue.
- *Ferram Aerospace Research (FAR)*. May spam logs with `NullPointerException` error, other consequences are unknown. As for now it's unknown if it's KIS or FAR issue. There is no ETA to fix it.