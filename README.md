---- Minecraft Crash Report ----
// Shall we play a game?

Time: 2026-08-17 01:04:08
Description: Unexpected error

org.spongepowered.asm.mixin.transformer.throwables.MixinTransformerError: An unexpected critical error was encountered
	at org.spongepowered.asm.mixin.transformer.MixinProcessor.applyMixins(MixinProcessor.java:380) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinTransformer.transformClass(MixinTransformer.java:253) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at net.neoforged.fml.loading.mixin.FMLMixinClassProcessor.processClass(FMLMixinClassProcessor.java:96) ~[loader-11.0.16.jar:11.0] {}
	at net.neoforged.fml.classloading.transformation.ClassTransformer.transform(ClassTransformer.java:96) ~[loader-11.0.16.jar:11.0] {}
	at net.neoforged.fml.classloading.transformation.TransformingClassLoader.maybeTransformClassBytes(TransformingClassLoader.java:47) ~[loader-11.0.16.jar:11.0] {}
	at net.neoforged.fml.classloading.ModuleClassLoader.readerToClass(ModuleClassLoader.java:224) ~[loader-11.0.16.jar:11.0] {}
	at net.neoforged.fml.classloading.ModuleClassLoader.loadClass(ModuleClassLoader.java:245) ~[loader-11.0.16.jar:11.0] {}
	at java.base/java.lang.ClassLoader.loadClass(ClassLoader.java:490) ~[?:?] {}
	at TRANSFORMER/sodium@0.9.2-alpha.4+mc26.2/net.caffeinemc.mods.sodium.client.render.chunk.RenderSectionManager.<init>(RenderSectionManager.java:142) ~[net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.2-mod.jar:?] {neoforge:mixin[APP:mixins.iris.compat.sodium.json:MixinRenderSectionManager from mod iris,APP:mixins.iris.compat.sodium.json:MixinRenderSectionManagerShadow from mod iris]}
	at TRANSFORMER/sodium@0.9.2-alpha.4+mc26.2/net.caffeinemc.mods.sodium.client.render.SodiumWorldRenderer.initRenderer(SodiumWorldRenderer.java:329) ~[net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.2-mod.jar:?] {neoforge:mixin[APP:mixins.iris.compat.sodium.json:MixinSodiumWorldRenderer from mod iris]}
	at TRANSFORMER/sodium@0.9.2-alpha.4+mc26.2/net.caffeinemc.mods.sodium.client.render.SodiumWorldRenderer.loadLevel(SodiumWorldRenderer.java:132) ~[net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.2-mod.jar:?] {neoforge:mixin[APP:mixins.iris.compat.sodium.json:MixinSodiumWorldRenderer from mod iris]}
	at TRANSFORMER/sodium@0.9.2-alpha.4+mc26.2/net.caffeinemc.mods.sodium.client.render.SodiumWorldRenderer.setLevel(SodiumWorldRenderer.java:125) ~[net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.2-mod.jar:?] {neoforge:mixin[APP:mixins.iris.compat.sodium.json:MixinSodiumWorldRenderer from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.renderer.extract.LevelExtractor.handler$zzn000$sodium$setRenderer(LevelExtractor.java:655) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:sodium-common.mixins.json:core.render.world.LevelExtractorMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.LevelExtractorMixin from mod sodium,APP:mixins.iris.json:MixinLevelRenderer_SkipRendering from mod iris,APP:mixins.iris.json:fabulous.MixinDisableFabulousGraphics from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.renderer.extract.LevelExtractor.setLevel(LevelExtractor.java:422) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:sodium-common.mixins.json:core.render.world.LevelExtractorMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.LevelExtractorMixin from mod sodium,APP:mixins.iris.json:MixinLevelRenderer_SkipRendering from mod iris,APP:mixins.iris.json:fabulous.MixinDisableFabulousGraphics from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.updateLevelInEngines(Minecraft.java:2274) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.updateLevelInEngines(Minecraft.java:2264) [minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.setLevel(Minecraft.java:2128) [minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.multiplayer.ClientPacketListener.handleLogin(ClientPacketListener.java:521) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:access_transformer,neoforge:access_transformer,neoforge:mixin[APP:sodium-common.mixins.json:core.world.map.ClientPacketListenerMixin from mod sodium,APP:mixins.iris.json:MixinClientPacketListener from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.network.protocol.game.ClientboundLoginPacket.handle(ClientboundLoginPacket.java:70) ~[minecraft-client-patched-26.2.0.59.jar:?] {}
	at TRANSFORMER/minecraft@26.2/net.minecraft.network.protocol.game.ClientboundLoginPacket.handle(ClientboundLoginPacket.java:14) ~[minecraft-client-patched-26.2.0.59.jar:?] {}
	at TRANSFORMER/minecraft@26.2/net.minecraft.network.PacketProcessor$ListenerAndPacket.handle(PacketProcessor.java:66) ~[minecraft-client-patched-26.2.0.59.jar:?] {}
	at TRANSFORMER/minecraft@26.2/net.minecraft.network.PacketProcessor.processQueuedPackets(PacketProcessor.java:52) ~[minecraft-client-patched-26.2.0.59.jar:?] {}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.runTick(Minecraft.java:1191) [minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.run(Minecraft.java:928) [minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.main.Main.main(Main.java:294) [minecraft-client-patched-26.2.0.59.jar:?] {}
	at net.neoforged.fml.startup.Client.main(Client.java:19) [loader-11.0.16.jar:11.0] {}
	at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:104) ~[?:?] {}
	at java.base/java.lang.reflect.Method.invoke(Method.java:565) ~[?:?] {}
	at io.github.zekerzhayard.forgewrapper.installer.Main.main(Main.java:67) [ForgeWrapper-prism-2026-08-01.jar:prism-2026-08-01] {}
	at org.prismlauncher.launcher.impl.StandardLauncher.launch(StandardLauncher.java:115) [NewLaunch.jar:?] {}
	at org.prismlauncher.EntryPoint.listen(EntryPoint.java:129) [NewLaunch.jar:?] {}
	at org.prismlauncher.EntryPoint.main(EntryPoint.java:70) [NewLaunch.jar:?] {}
Caused by: org.spongepowered.asm.mixin.injection.throwables.InjectionError: Critical injection failure: Redirector iris$forceClear(Lnet/caffeinemc/mods/sodium/client/render/chunk/region/RenderRegion;)V in mixins.iris.compat.sodium.json:MixinRenderRegionManager from mod iris failed injection check, (0/1) succeeded. Scanned 0 target(s). No refMap loaded.
	at org.spongepowered.asm.mixin.injection.struct.InjectionInfo.postInject(InjectionInfo.java:531) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinTargetContext.applyInjections(MixinTargetContext.java:1477) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinApplicatorStandard.applyInjections(MixinApplicatorStandard.java:832) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinApplicatorStandard.lambda$runApplicatorPass$7(MixinApplicatorStandard.java:362) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinApplicatorStandard.processMixins(MixinApplicatorStandard.java:381) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinApplicatorStandard.runApplicatorPass(MixinApplicatorStandard.java:360) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinApplicatorStandard.apply(MixinApplicatorStandard.java:240) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.TargetClassContext.apply(TargetClassContext.java:437) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.TargetClassContext.applyMixins(TargetClassContext.java:418) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinProcessor.applyMixins(MixinProcessor.java:351) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	... 31 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Render thread
Stacktrace:
	at org.spongepowered.asm.mixin.transformer.MixinProcessor.applyMixins(MixinProcessor.java:380) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at org.spongepowered.asm.mixin.transformer.MixinTransformer.transformClass(MixinTransformer.java:253) ~[sponge-mixin-0.17.3+mixin.0.8.7.jar:0.17.3+mixin.0.8.7] {}
	at net.neoforged.fml.loading.mixin.FMLMixinClassProcessor.processClass(FMLMixinClassProcessor.java:96) ~[loader-11.0.16.jar:11.0] {}
	at net.neoforged.fml.classloading.transformation.ClassTransformer.transform(ClassTransformer.java:96) ~[loader-11.0.16.jar:11.0] {}
	at net.neoforged.fml.classloading.transformation.TransformingClassLoader.maybeTransformClassBytes(TransformingClassLoader.java:47) ~[loader-11.0.16.jar:11.0] {}
	at net.neoforged.fml.classloading.ModuleClassLoader.readerToClass(ModuleClassLoader.java:224) ~[loader-11.0.16.jar:11.0] {}
	at net.neoforged.fml.classloading.ModuleClassLoader.loadClass(ModuleClassLoader.java:245) ~[loader-11.0.16.jar:11.0] {}
	at java.base/java.lang.ClassLoader.loadClass(ClassLoader.java:490) ~[?:?] {}
	at TRANSFORMER/sodium@0.9.2-alpha.4+mc26.2/net.caffeinemc.mods.sodium.client.render.chunk.RenderSectionManager.<init>(RenderSectionManager.java:142) ~[net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.2-mod.jar:?] {neoforge:mixin[APP:mixins.iris.compat.sodium.json:MixinRenderSectionManager from mod iris,APP:mixins.iris.compat.sodium.json:MixinRenderSectionManagerShadow from mod iris]}
	at TRANSFORMER/sodium@0.9.2-alpha.4+mc26.2/net.caffeinemc.mods.sodium.client.render.SodiumWorldRenderer.initRenderer(SodiumWorldRenderer.java:329) ~[net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.2-mod.jar:?] {neoforge:mixin[APP:mixins.iris.compat.sodium.json:MixinSodiumWorldRenderer from mod iris]}
	at TRANSFORMER/sodium@0.9.2-alpha.4+mc26.2/net.caffeinemc.mods.sodium.client.render.SodiumWorldRenderer.loadLevel(SodiumWorldRenderer.java:132) ~[net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.2-mod.jar:?] {neoforge:mixin[APP:mixins.iris.compat.sodium.json:MixinSodiumWorldRenderer from mod iris]}
	at TRANSFORMER/sodium@0.9.2-alpha.4+mc26.2/net.caffeinemc.mods.sodium.client.render.SodiumWorldRenderer.setLevel(SodiumWorldRenderer.java:125) ~[net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.2-mod.jar:?] {neoforge:mixin[APP:mixins.iris.compat.sodium.json:MixinSodiumWorldRenderer from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.renderer.extract.LevelExtractor.handler$zzn000$sodium$setRenderer(LevelExtractor.java:655) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:sodium-common.mixins.json:core.render.world.LevelExtractorMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.LevelExtractorMixin from mod sodium,APP:mixins.iris.json:MixinLevelRenderer_SkipRendering from mod iris,APP:mixins.iris.json:fabulous.MixinDisableFabulousGraphics from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.renderer.extract.LevelExtractor.setLevel(LevelExtractor.java:422) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:sodium-common.mixins.json:core.render.world.LevelExtractorMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.LevelExtractorMixin from mod sodium,APP:mixins.iris.json:MixinLevelRenderer_SkipRendering from mod iris,APP:mixins.iris.json:fabulous.MixinDisableFabulousGraphics from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.updateLevelInEngines(Minecraft.java:2274) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.updateLevelInEngines(Minecraft.java:2264) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.setLevel(Minecraft.java:2128) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.multiplayer.ClientPacketListener.handleLogin(ClientPacketListener.java:521) ~[minecraft-client-patched-26.2.0.59.jar:?] {neoforge:access_transformer,neoforge:access_transformer,neoforge:mixin[APP:sodium-common.mixins.json:core.world.map.ClientPacketListenerMixin from mod sodium,APP:mixins.iris.json:MixinClientPacketListener from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.network.protocol.game.ClientboundLoginPacket.handle(ClientboundLoginPacket.java:70) ~[minecraft-client-patched-26.2.0.59.jar:?] {}
	at TRANSFORMER/minecraft@26.2/net.minecraft.network.protocol.game.ClientboundLoginPacket.handle(ClientboundLoginPacket.java:14) ~[minecraft-client-patched-26.2.0.59.jar:?] {}
	at TRANSFORMER/minecraft@26.2/net.minecraft.network.PacketProcessor$ListenerAndPacket.handle(PacketProcessor.java:66) ~[minecraft-client-patched-26.2.0.59.jar:?] {}
-- Uptime --
Details:
	JVM uptime: 29.236s
	Wall uptime: 19.599s
	High-res time: 27.771s
	Client ticks: 178 ticks / 8.900s
Stacktrace:
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.fillReport(Minecraft.java:2446) [minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.emergencySaveAndCrash(Minecraft.java:975) [minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.Minecraft.run(Minecraft.java:951) [minecraft-client-patched-26.2.0.59.jar:?] {neoforge:mixin[APP:mixins.iris.json:MixinOptions_Entrypoint from mod iris,APP:sodium-common.mixins.json:core.MinecraftMixin from mod sodium,APP:sodium-common.mixins.json:features.gui.hooks.debug.MinecraftRenderFrameMixin from mod sodium,APP:sodium-neoforge.mixins.json:platform.neoforge.EntrypointMixin from mod sodium,APP:mixins.iris.json:MixinMinecraft_Images from mod iris,APP:mixins.iris.json:MixinMinecraft_Keybinds from mod iris,APP:mixins.iris.json:MixinMinecraft_PipelineManagement from mod iris]}
	at TRANSFORMER/minecraft@26.2/net.minecraft.client.main.Main.main(Main.java:294) [minecraft-client-patched-26.2.0.59.jar:?] {}
	at net.neoforged.fml.startup.Client.main(Client.java:19) [loader-11.0.16.jar:11.0] {}
	at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:104) ~[?:?] {}
	at java.base/java.lang.reflect.Method.invoke(Method.java:565) ~[?:?] {}
	at io.github.zekerzhayard.forgewrapper.installer.Main.main(Main.java:67) [ForgeWrapper-prism-2026-08-01.jar:prism-2026-08-01] {}
	at org.prismlauncher.launcher.impl.StandardLauncher.launch(StandardLauncher.java:115) [NewLaunch.jar:?] {}
	at org.prismlauncher.EntryPoint.listen(EntryPoint.java:129) [NewLaunch.jar:?] {}
	at org.prismlauncher.EntryPoint.main(EntryPoint.java:70) [NewLaunch.jar:?] {}


-- Affected level --
Details:
	All players: 0 total;
	Chunk stats: 729, 0
	Level dimension: minecraft:overworld
	Level time: 0 game time, 0 day time
	Level spawn location: World: (8,64,8), Section: (at 8,0,8 in 0,4,0; chunk contains blocks 0,-64,0 to 15,319,15), Region: (0,0; contains chunks 0,0 to 31,31, blocks 0,-64,0 to 511,319,511)
	Server brand: ~~ERROR~~ NullPointerException: Cannot read field "connection" because "this.minecraft.player" is null
	Server type: Integrated singleplayer server
	Tracked entity count: 0
	Client weather: Raining: false, thundering: false

-- Last reload --
Details:
	Reload number: 1
	Reload reason: initial
	Finished: Yes
	Packs: vanilla, mod_resources, mod/sodium, mod/iris, mod/justcoordinates, mod/ferritecore, mod/neoforge

-- System Details --
Details:
	Minecraft Version: 26.2
	Minecraft Version ID: 26.2
	Operating System: Linux (amd64) version 6.18.44_1
	Java Version: 25.0.2, Void
	Java VM Version: OpenJDK 64-Bit Server VM (mixed mode, sharing), Void
	Memory: 501844624 bytes (478 MiB) / 1191182336 bytes (1136 MiB) up to 8589934592 bytes (8192 MiB)
	Memory (heap): init: 512MiB, used: 653MiB, committed: 1136MiB, max: 8192MiB
	Memory (non-head): init: 007MiB, used: 218MiB, committed: 221MiB, max: 000MiB
	CPUs: 12
	Processor Vendor: AuthenticAMD
	Processor Name: AMD Ryzen 5 5500U with Radeon Graphics
	Identifier: AuthenticAMD Family 23 Model 104 Stepping 1
	Microarchitecture: unknown
	Frequency (GHz): -0.00
	Number of physical packages: 1
	Number of physical CPUs: 6
	Number of logical CPUs: 12
	Graphics card #0 name: Lucienne
	Graphics card #0 vendor: Advanced Micro Devices, Inc. [AMD/ATI] (0x1002)
	Graphics card #0 VRAM (MiB): 258.00
	Graphics card #0 deviceId: 0x164c
	Graphics card #0 versionInfo: unknown
	Virtual memory max (MiB): 31951.27
	Virtual memory used (MiB): 4459.82
	Swap memory total (MiB): 24549.00
	Swap memory used (MiB): 0.00
	Space in storage for jna.tmpdir (MiB): <path not set>
	Space in storage for org.lwjgl.system.SharedLibraryExtractPath (MiB): <path not set>
	Space in storage for io.netty.native.workdir (MiB): <path not set>
	Space in storage for java.io.tmpdir (MiB): available: 7353.15, total: 7402.27
	Space in storage for workdir (MiB): available: 182926.44, total: 233645.63
	Operating System Version: GNU/Linux Void unknown (unknown) build 6.18.44_1
	Process Elevated: false
	Process Loads: Uptime: 29s, user: 102s (354.06%), kernel: 6s (20.19%), total: 108s (374.25%)
	Process Virtual Size (MiB): 17652.86
	Process Resident Size (MiB): 2125.95
	JVM Flags: 2 total; -Xms512m -Xmx8192m
	Debug Flags: 0 total;
	Loaded Shaderpack: ComplementaryReimagined_r5.8.1.zip
		Profile: POTATO (+0 options changed by user)
	Launched Version: 26.2
	Launcher name: PrismLauncher
	Backend library: LWJGL version 3.4.1+2
	Window size: 958x523
	Surface Info: FIFO, 958 x 523
	GFLW Platform: x11
	Graphics Device: AMD Radeon Graphics (radeonsi, renoir, ACO, DRM 3.64, 6.18.44_1)
	Graphics Backend: OpenGL
	Graphics Vendor: AMD
	Graphics Drivers: 4.6 (Core Profile) Mesa 26.1.7
	Graphics Device Extensions: GL_ARB_multi_draw_indirect, GL_ARB_buffer_storage, GL_ARB_shader_draw_parameters, GL_ARB_base_instance, GL_KHR_debug, GL_ARB_draw_indirect, GL_ARB_clip_control, GL_ARB_vertex_attrib_binding, GL_ARB_direct_state_access, GL_EXT_texture_filter_anisotropic
	Graphics Device Type: OTHER
	Graphics Device Features: DeviceFeatures[shaderDrawParameters=true, multiDrawDirectInterleaved=false, multiDrawDirectSeparate=true, multiDrawIndirect=true, drawIndirect=true, nonZeroFirstInstance=true, persistentMapping=true]
	GL debug messages:
	Is Modded: Definitely; Client brand changed to 'neoforge'
	Universe: 400921fb54442d18
	Type: Client
	Transparency: regular
	Render Distance: 10/10 chunks
	Narrator config: OFF
	Narrator status: true
	Resource Packs: vanilla, mod_resources, mod/sodium, mod/iris, mod/justcoordinates, mod/ferritecore (incompatible), mod/neoforge (incompatible)
	Sound Cache: 48816 bytes in 1 buffers
	Current Language: en_us
	Locale: en_US
	System encoding: UTF-8
	File encoding: UTF-8
	CPU: 12x AMD Ryzen 5 5500U with Radeon Graphics
	Server Running: true
	Player Count: 1 / 8; [ServerPlayer['k1rak1ra'/95, l='ServerLevel[minecraft]', x=-106.69, y=87.00, z=51.27]]
	Active Data Packs: vanilla, mod_data, mod/sodium, mod/iris, mod/justcoordinates, mod/ferritecore (incompatible), mod/neoforge
	Available Data Packs: minecart_improvements, redstone_experiments, trade_rebalance, vanilla, mod/ferritecore (incompatible), mod/iris, mod/justcoordinates, mod/neoforge, mod/sodium, mod_data
	Enabled Feature Flags: minecraft:vanilla
	World Generation: Stable
	World Seed: -6063649602571078455
	Suppressed Exceptions: ~~NONE~~
	Type: Integrated Server
	Is Modded: Definitely; Client brand changed to 'neoforge'; Server brand changed to 'neoforge'
	Launched Version: 26.2
	Class Processors:
		00.00%: neoforge:computing_frames (marker)
		00.00%: neoforge:runtime_enum_extender
		04.38%: neoforge:access_transformer
		02.13%: neoforge:mixin
		00.00%: neoforge:simple_processors_default (marker)
		00.01%: neoforge.coremods:field_to_getter.net.minecraft.world.level.biome.biome
		00.01%: neoforge.coremods:field_to_getter.net.minecraft.world.level.block.flowerpotblock
		00.01%: neoforge.coremods:field_to_getter.net.minecraft.world.level.levelgen.structure.structure
		00.24%: neoforge.coremods:method_redirector
	Mod List:
		ferritecore-9.0.0-neoforge.jar                    |Ferrite Core                  |ferritecore                   |9.0.0               |Manifest: a3292dadb1caf7ad220d3a4b68abff2ad58592ddd372160f9cf66c57d159b539
		iris-neoforge-1.11.2+mc26.2.jar                   |Iris                          |iris                          |1.11.2+mc26.2       |Manifest: d30e423e9bc052301a8f98c8043e2af27ca9bda1e11538e550074b4da5c8d69e
		justcoordinates-0.7.0+26.2-neoforge.jar           |Just Coordinates              |justcoordinates               |0.7.0               |Manifest: 3a4aa870d6aeb60c3c536d3b54f954567a03931bff299e94614f8ca22ce98fec
		minecraft-client-patched-26.2.0.59.jar            |Minecraft                     |minecraft                     |26.2                |Manifest: b213c0c1235912c342089a53bbb5290d8eef4942f2b717c40a4a372915e021b6
		neoforge-26.2.0.59-universal.jar                  |NeoForge                      |neoforge                      |26.2.0.59           |Manifest: a924b85bdc145c04078ac2b9b2d2f271efb995a96f09830a12f4cffb23ee55d2
		net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.|Sodium                        |sodium                        |0.9.2-alpha.4+mc26.2|Manifest: 10c6a3e76bb4e00e38fd6e4502beaf63698fa50b990f017e371405505696582c
	Crash Report UUID: 77f2c73f-db11-4d1e-8c97-4abd72f0e296
	FML: 11.0.16
	NeoForge: 26.2.0.59
	Class Processors:
		00.00%: neoforge:computing_frames (marker)
		00.00%: neoforge:runtime_enum_extender
		04.38%: neoforge:access_transformer
		02.13%: neoforge:mixin
		00.00%: neoforge:simple_processors_default (marker)
		00.01%: neoforge.coremods:field_to_getter.net.minecraft.world.level.biome.biome
		00.01%: neoforge.coremods:field_to_getter.net.minecraft.world.level.block.flowerpotblock
		00.01%: neoforge.coremods:field_to_getter.net.minecraft.world.level.levelgen.structure.structure
		00.24%: neoforge.coremods:method_redirector
	Mod List:
		ferritecore-9.0.0-neoforge.jar                    |Ferrite Core                  |ferritecore                   |9.0.0               |Manifest: a3292dadb1caf7ad220d3a4b68abff2ad58592ddd372160f9cf66c57d159b539
		iris-neoforge-1.11.2+mc26.2.jar                   |Iris                          |iris                          |1.11.2+mc26.2       |Manifest: d30e423e9bc052301a8f98c8043e2af27ca9bda1e11538e550074b4da5c8d69e
		justcoordinates-0.7.0+26.2-neoforge.jar           |Just Coordinates              |justcoordinates               |0.7.0               |Manifest: 3a4aa870d6aeb60c3c536d3b54f954567a03931bff299e94614f8ca22ce98fec
		minecraft-client-patched-26.2.0.59.jar            |Minecraft                     |minecraft                     |26.2                |Manifest: b213c0c1235912c342089a53bbb5290d8eef4942f2b717c40a4a372915e021b6
		neoforge-26.2.0.59-universal.jar                  |NeoForge                      |neoforge                      |26.2.0.59           |Manifest: a924b85bdc145c04078ac2b9b2d2f271efb995a96f09830a12f4cffb23ee55d2
		net.caffeinemc.sodium-neoforge-0.9.2-alpha.4+mc26.|Sodium                        |sodium                        |0.9.2-alpha.4+mc26.2|Manifest: 10c6a3e76bb4e00e38fd6e4502beaf63698fa50b990f017e371405505696582c
	Crash Report UUID: 73938260-71a9-4cb3-9326-690743cc9ebd
	FML: 11.0.16
	NeoForge: 26.2.0.59
