INPUT := gfx/conback.lmp \
	gfx/mainmenu2.lmp \
	gfx/p_mods.lmp \
	maps/e1m1@c49d.ent \
	maps/e1m2@0caa.ent \
	maps/e1m4@958e.ent \
	maps/e2m2@fbfe.ent \
	maps/e2m3@237a.ent \
	maps/e2m7@10a8.ent \
	default.cfg

OUTPUT := vkquake.pak

$(OUTPUT): $(INPUT)
	cc mkpak.c -o mkpak --std=gnu11 -g && ./mkpak $(OUTPUT) $(INPUT)

.PHONY: clean
clean:
	rm -f $(OUTPUT)
	rm -f mkpak

