srpm:
	dnf install -y rpmdevtools
	spectool --get-files --directory $(outdir) $(spec)
	rpmbuild \
	--define "_sourcedir $(outdir)" \
	--define "_srcrpmdir $(outdir)" \
	-bs $(spec)