# $FreeBSD$

PACKAGE=	tests

TESTSDIR=       ${TESTSBASE}/sys/netpfil/pf
TESTS_SUBDIRS+=	ioctl

ATF_TESTS_SH+=	altq \
		anchor \
		pass_block \
		checksum \
		ether \
		forward \
		fragmentation \
		get_state \
		icmp \
		killstate \
		macro \
		map_e \
		match \
		names \
		nat \
		rules_counter \
		set_tos \
		src_track \
		rdr \
		ridentifier \
		route_to \
		syncookie \
		synproxy \
		set_skip \
		pfsync \
		proxy \
		table \
		tos

ATF_TESTS_SH+=	\
	pfsense_match

${PACKAGE}FILES+=	utils.subr \
			daytime_inetd.conf \
			echo_inetd.conf \
			CVE-2019-5597.py \
			CVE-2019-5598.py \
			fragcommon.py \
			frag-overindex.py \
			frag-overlimit.py \
			frag-overreplace.py \
			pfsync_defer.py

${PACKAGE}FILESMODE_CVE-2019-5597.py=	0555
${PACKAGE}FILESMODE_CVE-2019-5598.py=	0555
${PACKAGE}FILESMODE_fragcommon.py=	0555
${PACKAGE}FILESMODE_frag-overindex.py=	0555
${PACKAGE}FILESMODE_frag-overlimit.py=	0555
${PACKAGE}FILESMODE_frag-overreplace.py=	0555
${PACKAGE}FILESMODE_pfsync_defer.py=	0555

.include <bsd.test.mk>
