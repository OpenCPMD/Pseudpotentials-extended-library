**********************************************************************************
********                     WARNING AND DISCLAIMER                      *********
**********************************************************************************

The following list is comprehensive of all the pseudopotentials provided
in the present extended library package. In each case, the reported ECUT
value has to be intended only as the MINIMAL plane-wave cut-off needed to
get meaningful results.
In case of non-linear core corrections (NLCC) the keyword NLCC must be
included in the CPMD input file, section &ATOMS ... &END on the line where
the PP is written. Example:
*Mg_MT_HCTH_NLCC.psp  KLEINMAN-BYLANDER NLCC
 LMAX=P LOC=S
 ...

A legend for the short-hand notations used to name the pseudopotentials
is given at the bottom of the present file.

ELEMENT  PP TYPE                          NAME                    USAGE                      REFERENCES

  H      LDA BHS                          H_BHS_LDA.psp           LMAX=S LOC=S ECUT=25 Ry     [1]
  H      LDA MT (Ballone)                 H_MT_LDA.psp            LMAX=S LOC=S ECUT=25 Ry     [2]
  H      BP MT (Boero)                    H_MT_BP.psp             LMAX=S LOC=S ECUT=25 Ry    [15]
  H      PW91 MT (Boero-Rousseau)         H_MT_PW91.psp           LMAX=S LOC=S ECUT=25 Ry
  H      BLYP MT (Boero)                  H_MT_BLYP.psp           LMAX=S LOC=S ECUT=25 Ry     [3]
  H      PBE MT (Rousseau)                H_MT_PBE.psp            LMAX=S LOC=S ECUT=25 Ry     [4]
  H      revPBE MT (Boero)                H_MT_revPBE.psp         LMAX=S LOC=S ECUT=25 Ry
  H      HCTH MT (Boero)                  H_MT_HCTH.psp           LMAX=S LOC=S ECUT=25 Ry     [5]
  H      OLYP MT (Boero)                  H_MT_OLYP.psp           LMAX=S LOC=S ECUT=25 Ry
  H      XLYP MT (Hutter)                 H_MT_XLYP.psp           LMAX=S LOC=S ECUT=25 Ry
  H      LDA GTH (Goedecker)              H_GTH_LDA.psp           LMAX=S LOC=S ECUT=30 Ry     [6]
  H      BLYP GTH (Goedecker)             H_GTH_BLYP.psp          LMAX=S LOC=S ECUT=30 Ry     [6]
  H      PBE CVB (Giannozzi)              H_CVB_PBE.psp           LMAX=S LOC=S ECUT=20 Ry
  H      HCTH CVB                         H_CVB_HCTH.psp          LMAX=S LOC=S ECUT=20 Ry
  H      BLYP CVB (Giannozzi)             H_SPRIK_BLYP.psp        LMAX=S LOC=S ECUT=20 Ry     [7]
  H      PBE USPP-Vanderbilt (Ikeda)      001-H-gpbe-bm.uspp      LMAX=S LOC=S ECUT=18 Ry
  H      BLYP USPP-Vanderbilt (Boero)     H_blyp_ps.uspp          LMAX=S LOC=S ECUT=18 Ry
  H      BLYP USPP-Vanderbilt(Ikeda-Boero)H_VDB_BLYP.psp          LMAX=S LOC=S ECUT=18 Ry
  H      LDA (Giannozzi special use only) H_MT_PZ075-UPF.psp      LMAX=S LOC=S ECUT=20 Ry     [60]
  H      LDA (Giannozzi special use only) H_MT_PZ125-UPF.psp      LMAX=S LOC=S ECUT=20 Ry     [60]
  H      PBE (Boero special use only)     H_MT_PBE075.psp         LMAX=S LOC=S ECUT=20 Ry     [61]
  H      PBE (Boero special use only)     H-q1_GTH_PBE.psp        LMAX=S LOC=S ECUT=40 Ry
  He     PBE GTH (Ikeda-Boero)            He-q2_GTH_PBE.psp       LMAX=S LOC=S ECUT=40 Ry
  He     revPBE GTH (Ikeda-Boero)         He-q2_GTH_revPBE.psp    LMAX=S LOC=S ECUT=40 Ry
  He     BLYP GTH (Ikeda-Boero)           He-q2_GTH_BLYP.psp      LMAX=S LOC=S ECUT=40 Ry
  He     HCTH GTH (Ikeda-Boero)           He-q2_GTH_HCTH.psp      LMAX=S LOC=S ECUT=40 Ry
  Li     LDA SGS                          Li_SGS_LDA.psp          LMAX=S LOC=S ECUT=35 Ry     [1]
  Li     LDA MT NLCC (Giannozzi)          Li_MT_GIA_NLCC.psp      LMAX=S LOC=S ECUT=35 Ry     [8]
  Li     Becke Only NLCC (Rousseau)       Li_MT_BONLY_NLCC.psp    LMAX=S LOC=S ECUT=15 Ry     [9]
  Li     BLYP MT NLCC (Boero-Oshikiri)    Li_MT_BLYP_NLCC.psp     LMAX=S LOC=S ECUT=35 Ry    [10]
  Li     LDA GTH (Goedecker)              Li_GTH_LDA.psp          LMAX=S LOC=S ECUT=35 Ry     [6]
  Li     PBE GTH (Krack)                  Li_GTH_PBE.psp          LMAX=S LOC=S ECUT=35 Ry     [9]
  Li     BLYP GTH (Krack)                 Li_GTH_BLYP.psp         LMAX=S LOC=S ECUT=35 Ry     [9]
  Be     LDA SGS                          Be_SGS_LDA.psp          LMAX=P LOC=P ECUT=25 Ry     [1]
  Be     LDA GTH (Goedecker)              Be_GTH_LDA.psp          LMAX=P LOC=P ECUT=30 Ry     [6]
  Be     BLYP GTH (Goedecker)             Be_GTH_BLYP.psp         LMAX=P LOC=P ECUT=30 Ry     [6]
  B      LDA SGS                          B_SGS_LDA.psp           LMAX=P LOC=P ECUT=20 Ry     [1]
  B      BP MT (Boero)                    B_MT_BP.psp             LMAX=P LOC=P ECUT=25 Ry    [11]
  B      PBE MT (Boero)                   B_MT_PBE.psp            LMAX=P LOC=P ECUT=25 Ry    [11]
  B      revPBE MT (Boero)                B_MT_revPBE.psp         LMAX=P LOC=P ECUT=25 Ry    [11]
  B      BLYP MT (Boero)                  B_MT_BLYP.psp           LMAX=P LOC=P ECUT=25 Ry    [11]
  B      HCTH MT (Boero)                  B_MT_HCTH.psp           LMAX=P LOC=P ECUT=25 Ry
  B      OLYP MT (Boero)                  B_MT_OLYP.psp           LMAX=P LOC=P ECUT=25 Ry
  B      LDA GTH (Goedecker)              B_GTH_LDA.psp           LMAX=P LOC=P ECUT=30 Ry     [6]
  B      BLYP GTH (Goedecker)             B_GTH_BLYP.psp          LMAX=P LOC=P ECUT=30 Ry     [6]
  C      LDA SGS                          C_SGS_LDA.psp           LMAX=P LOC=P ECUT=30 Ry     [1]
  C      LDA MT (Giannozzi-Dal Corso)     C_MT_GIA.psp            LMAX=P LOC=P ECUT=35 Ry    [12]
  C      BP MT (Giannozzi)                C_MT_GIA_BP.psp         LMAX=P LOC=P ECUT=35 Ry    [13]
  C      BP MT (Boero)                    C_MT_BP.psp             LMAX=P LOC=P ECUT=35 Ry
  C      BLYP MT (Giannozzi)              C_MT_GIA_BLYP.psp       LMAX=P LOC=P ECUT=35 Ry    [15]
  C      BLYP MT "hard" (Boero)           C_MT_BLYP_1.psp         LMAX=P LOC=P ECUT=40 Ry
  C      BLYP MT "soft" (Boero)           C_MT_BLYP_2.psp         LMAX=P LOC=P ECUT=30 Ry
  C      PW91 MT (Boero)                  C_MT_PW91.psp           LMAX=P LOC=P ECUT=40 Ry
  C      PBE MT (Boero)                   C_MT_PBE.psp            LMAX=P LOC=P ECUT=40 Ry
  C      revPBE MT (Boero)                C_MT_revPBE.psp         LMAX=P LOC=P ECUT=40 Ry
  C      HCTH MT (Boero)                  C_MT_HCTH.psp           LMAX=P LOC=P ECUT=40 Ry     [5]
  C      OLYP MT (Boero)                  C_MT_OLYP.psp           LMAX=P LOC=P ECUT=40 Ry
  C      XLYP MT (Boero)                  C_MT_XLYP.psp           LMAX=P LOC=P ECUT=40 Ry
  C      LDA GTH (Goedecker)              C_GTH_LDA.psp           LMAX=P LOC=P ECUT=40 Ry     [6]
  C      PBE GTH (Goedecker)              C_GTH_PBE.psp           LMAX=P LOC=P ECUT=40 Ry     [6]
  C      BLYP GTH (Goedecker)             C_GTH_BLYP.psp          LMAX=P LOC=P ECUT=40 Ry     [6]
  C      LDA MT-derived soft (Kunc)       C_SOFT_Kunc_LDA.psp     LMAX=P LOC=P ECUT=24 Ry    [14]
  C      PBE USPP-Vanderbilt (Ikeda)      006-C-gpbe-bm.uspp      LMAX=P LOC=P ECUT=24 Ry
  C      BLYP USPP-Vanderbilt (Boero)     C_blyp_ps.uspp          LMAX=P LOC=P ECUT=24 Ry
  C      BLYP USPP-Vanderbilt(Ikeda-Boero)C_VDB_BLYP.psp          LMAX=P LOC=P ECUT=24 Ry
  N      LDA SGS                          N_SGS_LDA.psp           LMAX=P LOC=P ECUT=40 Ry     [1]
  N      LDA MT (Giannozzi)               N_MT_GIA.psp            LMAX=P LOC=P ECUT=40 Ry
  N      BP MT  (Giannozzi)               N_MT_BP.psp             LMAX=P LOC=P ECUT=40 Ry
  N      BLYP MT (Raugei)                 N_MT_BLYP.psp           LMAX=P LOC=P ECUT=40 Ry
  N      PBE MT (Boero)                   N_MT_PBE.psp            LMAX=P LOC=P ECUT=40 Ry
  N      revPBE MT (Boero)                N_MT_revPBE.psp         LMAX=P LOC=P ECUT=40 Ry
  N      HCTH MT (Boero)                  N_MT_HCTH.psp           LMAX=P LOC=P ECUT=40 Ry    [38]
  N      OLYP MT (Boero)                  N_MT_OLYP.psp           LMAX=P LOC=P ECUT=40 Ry
  N      LDA GTH (Goedecker)              N_GTH_LDA.psp           LMAX=P LOC=P ECUT=70 Ry     [6]
  N      PBE GTH (Goedecker)              N_GTH_PBE.psp           LMAX=P LOC=P ECUT=70 Ry     [6]
  N      BLYP GTH (Goedecker)             N_GTH_BLYP.psp          LMAX=P LOC=P ECUT=70 Ry     [6]
  N      PBE USPP-Vanderbilt (Ikeda)      007-N-gpbe-bm.uspp      LMAX=P LOC=P ECUT=30 Ry
  N      BLYP USPP-Vanderbilt (Boero)     N_blyp_ps.uspp          LMAX=P LOC=P ECUT=30 Ry
  O      LDA SGS                          O_SGS_LDA.psp           LMAX=P LOC=P ECUT=70 Ry
  O      LDA MT (Giannozzi)               O_MT_GIA.psp            LMAX=P LOC=P ECUT=70 Ry
  O      LDA MT                           O_MT_LDA.psp            LMAX=P LOC=P ECUT=70 Ry
  O      BLYP MT (Sprik-Giannozzi)        O_SPRIK_BLYP.psp        LMAX=P LOC=P ECUT=70 Ry     [8]
  O      revPBE MT (Boero)                O_MT_revPBE.psp         LMAX=P LOC=P ECUT=70 Ry
  O      HCTH MT (Boero)                  O_MT_HCTH.psp           LMAX=P LOC=P ECUT=70 Ry     [5]
  O      PBE MT (Boero)                   O_MT_PBE.psp            LMAX=P LOC=P ECUT=70 Ry
  O      BP  MT (Hutter)                  O_MT_BP.psp             LMAX=P LOC=P ECUT=70 Ry
  O      PW91 MT (Boero)                  O_MT_PW91.psp           LMAX=P LOC=P ECUT=70 Ry
  O      OLYP MT (Boero)                  O_MT_OLYP.psp           LMAX=P LOC=P ECUT=70 Ry
  O      XLYP MT (Hutter)                 O_MT_XLYP.psp           LMAX=P LOC=P ECUT=70 Ry
  O      GGA MT (Boero)                   O_MT_GGA.psp            LMAX=P LOC=P ECUT=70 Ry    [36]
  O      LDA GTH (Goedecker)              O_GTH_LDA.psp           LMAX=P LOC=P ECUT=70 Ry     [6]
  O      PBE GTH (Goedecker)              O_GTH_PBE.psp           LMAX=P LOC=P ECUT=70 Ry     [6]
  O      BLYP GTH (Goedecker)             O_GTH_BLYP.psp          LMAX=P LOC=P ECUT=70 Ry     [6]
  O      PBE USPP-Vanderbilt (Boero)      008-O-gpbe-bm.uspp      LMAX=P LOC=P ECUT=40 Ry
  O      BLYP USPP-Vanderbilt (Boero)     O_blyp_ps.uspp          LMAX=P LOC=P ECUT=40 Ry
  O      BLYP USPP-Vanderbilt(Ikeda-Boero)O_VDB_BLYP.psp          LMAX=P LOC=P ECUT=40 Ry
  F      LDA SGS                          F_SGS_LDA.psp           LMAX=P LOC=P ECUT=60 Ry
  F      BLYP MT (Raugei)                 F_MT_BLYP.psp           LMAX=P LOC=P ECUT=60 Ry
  F      BLYP MT (Boero-Grubmueller)      F_MT_BLYP2.psp          LMAX=D LOC=D ECUT=60 Ry
  F      HCTH MT (Boero-Grubmueller)      F_MT_HCTH.psp           LMAX=D LOC=D ECUT=60 Ry
  F      PBE MT (Boero-Grubmueller)       F_MT_PBE.psp            LMAX=D LOC=D ECUT=60 Ry
  F      OLYP MT (Boero )                 F_MT_OLYP.psp           LMAX=D LOC=D ECUT=60 Ry
  F      LDA GTH (Goedecker)              F_GTH_LDA.psp           LMAX=P LOC=P ECUT=60 Ry     [6]
  F      BLYP GTH (Goedecker)             F_GTH_BLYP.psp          LMAX=P LOC=P ECUT=60 Ry     [6]
  Ne     LDA SGS                          Ne_SGS_LDA.psp          LMAX=P LOC=P ECUT=40 Ry
  Na     LDA SGS                          Na_SGS_LDA.psp          LMAX=S LOC=S ECUT=50 Ry
  Na     LDA MT NLCC (Boero)              Na_MT_NLCC.psp          LMAX=S LOC=S ECUT=60 Ry
  Na     BLYP MT SEMI (Ramaniah)          Na_SEMI_BLYP.psp        LMAX=P LOC=S ECUT=80 Ry    [24]
  Na     HCTH MT SEMI (Boero-Costanzo)    Na_MT_HCTH_SEMI.psp     LMAX=P LOC=S ECUT=80 Ry    [41]
  Na     PBE MT SEMI (Boero)              Na_MT_PBE_SEMI.psp      LMAX=P LOC=S ECUT=80 Ry
  Na     XLYP MT SEMI (Boero)             Na_MT_XLYP_SEMI.psp     LMAX=P LOC=S ECUT=80 Ry
  Na     PW91 MT SEMI (Boero)             Na_MT_PW91_SEMI.psp     LMAX=P LOC=S ECUT=80 Ry
  Na     LDA GTH (Goedecker)              Na_GTH_LDA.psp          LMAX=S LOC=S ECUT=80 Ry     [6]
  Na     BLYP GTH (Goedecker)             Na_GTH_BLYP.psp         LMAX=S LOC=S ECUT=80 Ry     [6]
  Na     PBE Vanderbilt-USPP (Boero)      Na_USPP_PBE.psp         LMAX=S LOC=S ECUT=40 Ry ! Old VDB format !
  Mg     LDA SGS                          Mg_SGS_LDA.psp          LMAX=S LOC=S ECUT=40 Ry
  Mg     LDA HCTH                         Mg_SGS_HCTH.psp         LMAX=S LOC=S ECUT=40 Ry
  Mg     HCTH MT NLCC (Boero)             Mg_MT_HCTH_NLCC.psp     LMAX=P LOC=S ECUT=40 Ry     [5]
  Mg     BP MT NLCC (Boero)               Mg_MT_BP_NLCC.psp       LMAX=P LOC=S ECUT=40 Ry
  Mg     BLYP MT NLCC (Boero)             Mg_MT_BLYP_NLCC.psp     LMAX=P LOC=S ECUT=40 Ry
  Mg     BLYP MT NLCC soft (Boero)        Mg_MT_BLYP_NLCC2.psp    LMAX=P LOC=S ECUT=40 Ry
  Mg     BP MT SEMI (Boero)               Mg_MT_BP_SEMI.psp       LMAX=P LOC=P ECUT=80 Ry
  Mg     PBE MT SEMI (Boero)              Mg_MT_PBE_SEMI.psp      LMAX=P LOC=P ECUT=80 Ry
  Mg     revPBE MT SEMI (Boero-Ikeda)     Mg_MT_revPBE_SEMI.psp   LMAX=P LOC=P ECUT=80 Ry
  Mg     BLYP MT SEMI (Boero)             Mg_MT_BLYP_SEMI.psp     LMAX=P LOC=P ECUT=80 Ry
  Mg     HCTH MT SEMI (Boero)             Mg_MT_HCTH_SEMI.psp     LMAX=P LOC=P ECUT=80 Ry     [5]
  Mg     XLYP MT SEMI (Boero)             Mg_MT_XLYP_NLCC.psp     LMAX=P LOC=P ECUT=80 Ry
  Mg     PBE GTH SEMI (Ikeda)             Mg_GTH_PBE_SEMI.psp     LMAX=P LOC=P ECUT=80 Ry
  Mg     PBE MT NLCC (Celino)             Mg_MT_PBE_NLCC_FHI.psp  LMAX=S LOC=S ECUT=40 Ry
  Mg     LDA GTH (Goedecker)              Mg_GTH_LDA.psp          LMAX=S LOC=S ECUT=70 Ry     [6]
  Mg     BLYP GTH (Goedecker)             Mg_GTH_BLYP.psp         LMAX=S LOC=S ECUT=70 Ry     [6]
  Mg     PBE USPP-Vanderbilt (Boero)      012-Mg-gpbe-bm.uspp     LMAX=S LOC=S ECUT=20 Ry
  Mg     BLYP USPP-Vanderbilt (Boero)     012-Mg-blyp-bm.uspp     LMAX=S LOC=S ECUT=20 Ry
  Al     LDA SGS                          Al_SGS_LDA.psp          LMAX=P LOC=S ECUT=60 Ry
  Al     BLYP MT (Giannozzi)              Al_MT_GIA_BLYP.psp      LMAX=D LOC=S ECUT=60 Ry    [59]
  Al     BLYP MT NLCC (Giannozzi)         Al_MT_GIA_BLYP_NLCC.psp LMAX=D LOC=S ECUT=60 Ry    [59]
  Al     PW91 MT (Brazdova)               Al_MT_PW91.psp          LMAX=P LOC=S ECUT=80 Ry    [36]
  Al     GGA MT (Boero)                   Al_MT_GGA.psp           LMAX=P LOC=S ECUT=80 Ry
  Al     HCTH MT (Boero)                  Al_MT_HCTH.psp          LMAX=P LOC=S ECUT=80 Ry
  Al     XLYP MT (Boero)                  Al_MT_XLYP.psp          LMAX=P LOC=S ECUT=80 Ry
  Al     PBE MT (Seitsonen)               Al_MT_PBE.psp           LMAX=P LOC=S ECUT=80 Ry
  Al     revPBE MT (Boero-Ikeda)          Al_MT_revPBE.psp        LMAX=D LOC=D ECUT=80 Ry
  Al     LDA GTH (Goedecker)              Al_GTH_LDA.psp          LMAX=P LOC=P ECUT=80 Ry     [6]
  Al     BLYP GTH (Goedecker)             Al_GTH_BLYP.psp         LMAX=P LOC=P ECUT=80 Ry     [6]
  Al     PBE USPP-Vanderbilt (Ikeda)      013-Al-gpbe-ike.uspp    LMAX=P LOC=P ECUT=40 Ry
  Al     BLYP USPP-Vanderbilt (Boero)     Al_blyp_ps.uspp         LMAX=P LOC=P ECUT=40 Ry
  Si     LDA SGS                          Si_SGS_LDA.psp          LMAX=P LOC=P ECUT=16 Ry    [16]
  Si     PW CVB (Pasquarello-DalCorso)    Si_CVB_PW.psp           LMAX=D LOC=D ECUT=16 Ry    [44]
  Si     LDA MT                           Si_MT_LDA.psp           LMAX=D LOC=D ECUT=16 Ry    [17]
  Si     BP MT                            Si_MT_BP.psp            LMAX=D LOC=D ECUT=16 Ry    [18]
  Si     BLYP MT (Boero-Ikeda)            Si_MT_BLYP.psp          LMAX=D LOC=D ECUT=16 Ry
  Si     PBE MT (Boero)                   Si_MT_PBE.psp           LMAX=D LOC=D ECUT=16 Ry    [19]
  Si     revPBE MT (Boero-Ikeda)          Si_MT_revPBE.psp        LMAX=D LOC=D ECUT=16 Ry
  Si     HCTH MT (Ikeda-Boero)            Si_MT_HCTH.psp          LMAX=D LOC=D ECUT=16 Ry
  Si     OLYP MT (Boero)                  Si_MT_OLYP.psp          LMAX=D LOC=D ECUT=16 Ry
  Si     XLYP MT (Boero)                  Si_MT_XLYP.psp          LMAX=D LOC=D ECUT=16 Ry
  P      LDA SGS                          P_SGS_LDA.psp           LMAX=D LOC=S ECUT=40 Ry
  P      LDA MT (Trout)                   P_MT_LDA.psp            LMAX=D LOC=S ECUT=40 Ry
  P      BLYP MT (Boero)                  P_MT_BLYP.psp           LMAX=D LOC=S ECUT=40 Ry
  P      BLYP MT (Giannozzi)              P_MT_GIA_BLYP.psp       LMAX=D LOC=S ECUT=40 Ry
  P      PBE MT (Boero)                   P_MT_PBE.psp            LMAX=D LOC=S ECUT=40 Ry
  P      revPBE MT (Boero)                P_MT_revPBE.psp         LMAX=D LOC=S ECUT=40 Ry
  P      HCTH MT (Sprik)                  P_MT_SPR_HCTH.psp       LMAX=D LOC=S ECUT=40 Ry    [20]
  P      OLYP MT (Boero)                  P_MT_OLYP.psp           LMAX=D LOC=S ECUT=40 Ry
  P      XLYP MT (Boero)                  P_MT_XLYP.psp           LMAX=D LOC=S ECUT=40 Ry
  P      LDA GTH (Goedecker)              P_GTH_LDA.psp           LMAX=P LOC=P ECUT=50 Ry     [6]
  P      BLYP GTH (Goedecker)             P_GTH_BLYP.psp          LMAX=P LOC=P ECUT=50 Ry     [6]
  P      PBE USPP-Vanderbilt (Boero)      015-P-gpbe-bm.uspp      LMAX=P LOC=P ECUT=20 Ry
  P      BLYP USPP-Vanderbilt (Boero)     015-P-blyp-bm.uspp      LMAX=P LOC=P ECUT=20 Ry
  S      LDA SGS                          S_SGS_LDA.psp           LMAX=D LOC=D ECUT=35 Ry
  S      BP MT (Boero)                    S_MT_BP.psp             LMAX=D LOC=D ECUT=35 Ry
  S      BLYP MT (Rousseau)               S_MT_BLYP.psp           LMAX=D LOC=D ECUT=35 Ry     [4]
  S      PBE MT (Rousseau)                S_MT_PBE.psp            LMAX=D LOC=D ECUT=35 Ry
  S      revPBE MT (Boero)                S_MT_revPBE.psp         LMAX=D LOC=D ECUT=35 Ry
  S      HCTH MT (Ikeda)                  S_MT_HCTH.psp           LMAX=D LOC=D ECUT=35 Ry
  S      OLYP MT (Boero-Ikeda)            S_MT_OLYP.psp           LMAX=D LOC=D ECUT=35 Ry
  S      LDA GTH (Rousseau)               S_GTH_LDA.psp           LMAX=P LOC=P ECUT=40 Ry
  S      PBE GTH (Rousseau)               S_GTH_PBE.psp           LMAX=P LOC=P ECUT=40 Ry
  S      PBE USPP-Vanderbilt(Ikeda-Boero) S_VDB_PBE.psp           LMAX=P LOC=P ECUT=20 Ry
  Cl     LDA SGS                          Cl_SGS_LDA.psp          LMAX=P LOC=P ECUT=40 Ry
  Cl     LDA MT (Ballone)                 Cl_MT_LDA.psp           LMAX=P LOC=P ECUT=35 Ry     [3]
  Cl     BP MT (Ballone)                  Cl_MT_BP.psp            LMAX=P LOC=P ECUT=35 Ry
  Cl     BLYP MT (Boero)                  Cl_MT_BLYP.psp          LMAX=D LOC=D ECUT=35 Ry     [3]
  Cl     PBE MT (Boero)                   Cl_MT_PBE.psp           LMAX=D LOC=D ECUT=35 Ry
  Cl     revPBE MT (Boero)                Cl_MT_revPBE.psp        LMAX=D LOC=D ECUT=35 Ry
  Cl     HCTH MT (Boero)                  Cl_MT_HCTH.psp          LMAX=D LOC=D ECUT=35 Ry
  Cl     OLYP MT (Boero)                  Cl_MT_OLYP.psp          LMAX=D LOC=D ECUT=35 Ry
  Cl     LDA GTH (Goedecker)              Cl_GTH_LDA.psp          LMAX=P LOC=P ECUT=50 Ry
  Cl     BLYP GTH (Goedecker)             Cl_GTH_BLYP.psp         LMAX=P LOC=P ECUT=50 Ry
  Cl     PBE USPP-Vanderbilt (Ikeda)      017-Cl-gpbe-ike.uspp    LMAX=P LOC=P ECUT=24 Ry
  Cl     BLYP USPP-Vanderbilt (Boero)     Cl_blyp_ps.uspp         LMAX=P LOC=P ECUT=24 Ry
  Ar     LDA SGS                          Ar_SGS_LDA.psp          LMAX=P LOC=P ECUT=35 Ry
  Ar     BLYP MT (Boero-Ikeda)            Ar_MT_BLYP.psp          LMAX=P LOC=P ECUT=35 Ry
  Ar     PBE MT (Boero)                   Ar_MT_PBE.psp           LMAX=P LOC=P ECUT=35 Ry
  Ar     revPBE MT (Silvestrelli)         Ar_MT_revPBE.psp        LMAX=P LOC=P ECUT=35 Ry
  Ar     HCTH (Boero-Silvestrelli)        Ar_MT_HCTH.psp          LMAX=P LOC=P ECUT=35 Ry
  K      BLYP MT SEMI (Ramaniah-Boero)    K_MT_BLYP_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry    [25]
  K      HCTH MT SEMI (Boero-Ikeda)       K_MT_HCTH_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry    [40]
  K      PBE MT SEMI  (Boero-Ikeda)       K_MT_PBE_SEMI.psp       LMAX=D LOC=D ECUT=80 Ry
  K      BP MT SEMI  (Boero-Ikeda)        K_MT_BP_SEMI.psp        LMAX=D LOC=D ECUT=80 Ry
  K      XLYP MT SEMI (Boero)             K_MT_XLYP_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry
  K      PW91 MT SEMI (Boero)             K_MT_PW91_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry
  K      PBE GTH (Ikeda)                  K_GTH_PBE.psp           LMAX=P LOC=P ECUT=70 Ry
  K      HCTH GTH (Ikeda)                 K_GTH_HCTH.psp          LMAX=P LOC=P ECUT=70 Ry
  K      BLYP USPP-Vanderbilt (Boero)     019-K-blyp-bm.uspp      LMAX=P LOC=P ECUT=20 Ry
  Ca     BLYP MT SEMI (Giannozzi)         Ca_SEMI_BLYP_GIA.psp    LMAX=D LOC=S ECUT=80 Ry
  Ca     BLYP MT SEMI (Boero)             Ca_MT_BLYP_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry
  Ca     PW91 MT SEMI (Boero)             Ca_MT_PW91_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry
  Ca     PBE MT SEMI (Boero)              Ca_MT_PBE_SEMI.psp      LMAX=D LOC=S ECUT=80 Ry
  Ca     HCTH MT SEMI (Ikeda)             Ca_MT_HCTH_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry
  Sc     PBE GTH (Boero-Ikeda)            Sc_GTH_PBE.psp          LMAX=D LOC=D ECUT=80 Ry
  Ti     LDA MT NLCC  (Ballone)           Ti_MT_LDA_NLCC.psp      LMAX=D LOC=S SKIP=P ECUT=40 Ry  [3]
  Ti     PBE MT NLCC (Boero)              Ti_MT_PBE_NLCC.psp      LMAX=D LOC=S SKIP=P ECUT=40 Ry  [3]
  Ti     BLYP MT NLCC (Boero)             Ti_MT_BLYP_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=40 Ry  [3]
  Ti     HCTH MT NLCC (Boero)             Ti_MT_BLYP_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=40 Ry
  Ti     OLYP MT NLCC (Boero)             Ti_MT_OLYP_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=40 Ry
  Ti     BP GTH (Krack)                   Ti_GTH_BP.psp           LMAX=D LOC=D ECUT=80 Ry    [54]
  Ti     PBE GTH (Krack)                  Ti_GTH_PBE.psp          LMAX=D LOC=D ECUT=80 Ry    [54]
  Ti     BLYP GTH (Krack)                 Ti_GTH_BLYP.psp         LMAX=D LOC=D ECUT=80 Ry    [54]
  V      BLYP MT NLCC (Boero)             V_MT_BLYP_NLCC.psp      LMAX=D LOC=S SKIP=P ECUT=40 Ry
  V      BLYP MT NLCC (Giannozzi)         V_MT_GIA_BLYP_NLCC.psp  LMAX=D LOC=S ECUT=40 Ry
  V      PBE MT NLCC (Boero-Oshikiri)     V_MT_PBE_NLCC.psp       LMAX=D LOC=S ECUT=40 Ry    [57]
  V      BLYP MT SEMI (Boero-Odelius)     V_MT_SEMI_BLYP.psp      LMAX=D LOC=D ECUT=80 Ry    [21]
  V      HCTH MT SEMI (Boero)             V_MT_SEMI_HCTH.psp      LMAX=D LOC=D ECUT=80 Ry
  V      OLYP MT SEMI (Boero)             V_MT_SEMI_OLYP.psp      LMAX=D LOC=D ECUT=80 Ry
  V      PBE MT SEMI (Boero-Oshikiri)     V_MT_SEMI_PBE.psp       LMAX=D LOC=D ECUT=80 Ry
  V      GGA MT SEMI (Brazdova)           V_MT_GGA_SEMI.psp       LMAX=D LOC=D ECUT=80 Ry    [36]
  Cr     PBE MT SEMI (Boero)              Cr_MT_PBE_SEMI.psp      LMAX=D LOC=D ECUT=90 Ry
  Cr     BLYP MT SEMI (Boero)             Cr_MT_BLYP_SEMI.psp     LMAX=D LOC=D ECUT=90 Ry
  Cr     HCTH MT SEMI (Boero)             Cr_MT_HCTH_SEMI.psp     LMAX=D LOC=D ECUT=90 Ry
  Cr     OLYP MT SEMI (Boero)             Cr_MT_OLYP_SEMI.psp     LMAX=D LOC=D ECUT=90 Ry
  Cr     PBE GTH (Ikeda)                  Cr_GTH_PBE.psp          LMAX=D LOC=D ECUT=90 Ry
  Cr     PBE USPP-Vanderbilt (Boero)      024-Cr-gpbe-bm.uspp     LMAX=D LOC=D ECUT=50 Ry
  Mn     PBE MT NLCC (Ardevol-Rovira)     Mn_MT_PBE_NLCC.psp      LMAX=D LOC=S ECUT=60 Ry
  Mn     BLYP MT NLCC (Ardevol-Boero)     Mn_MT_BLYP_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=60 Ry
  Mn     HCTH MT NLCC (Ardevol-Boero)     Mn_MT_HCTH_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=60 Ry
  Mn     BLYP MT SEMI                     Mn_MT_SEMI_BLYP.psp     LMAX=D LOC=D or S ECUT=80 Ry
  Fe     LDA MT (Ballone)                 Fe_MT_LDA.psp           LMAX=D LOC=S ECUT=70 Ry    [22]
  Fe     BP MT NLCC (Ballone-Rovira)      Fe_MT_BP_NLCC.psp       LMAX=D LOC=S ECUT=70 Ry    [22]
  Fe     PBE MT NLCC (Boero-Rovira)       Fe_MT_PBE_NLCC.psp      LMAX=D LOC=S ECUT=70 Ry    [39]
  Fe     revPBE MT SEMI (Ikeda)           Fe_MT_revPBE_SEMI.psp   LMAX=D LOC=S ECUT=90 Ry
  Fe     BLYP MT NLCC (Massobrio)         Fe_MT_BLYP_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=80 Ry    [23]
  Fe     HCTH MT NLCC (Boero-Rovira)      Fe_MT_HCTH_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=80 Ry
  Fe     BP GTH (Rousseau)                Fe_GTH_BP.psp           LMAX=D LOC=S ECUT=80 Ry
  Fe     PBE GTH (Ikeda)                  Fe_GTH_PBE.psp          LMAX=D LOC=S ECUT=80 Ry
  Fe     BLYP GTH (Krack)                 Fe_GTH_BLYP_SEMI.psp    LMAX=D LOC=S ECUT=80 Ry    [54]
  Fe     PBE USPP-Vanderbilt (Ikeda-Boero)Fe_VDB_PBE_SEMI.psp     LMAX=D LOC=S ECUT=40 Ry
  Co     BP MT NLCC (Ballone)             Co_MT_BP_NLCC.psp       LMAX=D LOC=S SKIP=P ECUT=80 Ry    [42]
  Co     BLYP MT NLCC (Boero-Ballone)     Co_MT_BLYP_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=80 Ry
  Co     BLYP MT SEMI (Giannozzi)         Co_MT_GIA_BLYP_SEMI.psp LMAX=D LOC=S ECUT=90 Ry
  Co     PBE MT NLCC (Boero-Rovira)       Co_MT_PBE_NLCC.psp      LMAX=D LOC=S SKIP=P ECUT=80 Ry
  Co     HCTH MT NLCC (Boero-Rovira)      Co_MT_HCTH_NLCC.psp     LMAX=D LOC=S SKIP=P ECUT=80 Ry
  Co     PBE GTH (Krack)                  Co_GTH_PBE_SEMI.psp     LMAX=D LOC=S ECUT=90 Ry
  Co     BLYP GTH (Krack)                 Co_GTH_BLYP_SEMI.psp    LMAX=D LOC=S ECUT=90 Ry
  Ni     BLYP MT NLCC (Weiss)             Ni_MT_BLYP_NLCC.psp     LMAX=D LOC=S (or P) ECUT=80 Ry
  Ni     PW91 MT NLCC (Boero-Weiss)       Ni_MT_PW91_NLCC.psp     LMAX=D LOC=S (or P) ECUT=80 Ry
  Ni     PBE MT NLCC (Boero-Weiss)        Ni_MT_BLYP_NLCC.psp     LMAX=D LOC=S (or P) ECUT=80 Ry
  Ni     HCTH MT NLCC (Boero-Weiss)       Ni_MT_BLYP_NLCC.psp     LMAX=D LOC=S (or P) ECUT=80 Ry
  Ni     PBE GTH SEMI (Krack)             Ni_GTH_PBE_SEMI.psp     LMAX=D LOC=S (or P) ECUT=80 Ry
  Ni     BLYP GTH SEMI (Krack)            Ni_GTH_BLYP_SEMI.psp    LMAX=D LOC=S (or P) ECUT=80 Ry
  Cu     BP MT NLCC (Ballone)             Cu_MT_BP_NLCC.psp       LMAX=D LOC=S SKIP=P ECUT=70 Ry
  Cu     BLYP MT NLCC (Boero-Massobrio)   Cu_MT_BLYP_NLCC.psp     LMAX=D LOC=S ECUT=70 Ry    [34]
  Cu     PW91 MT NLCC (Boero-Oda)         Cu_MT_BLYP_NLCC.psp     LMAX=D LOC=S ECUT=70 Ry
  Cu     OLYP MT NLCC (Boero)             Cu_MT_OLYP_NLCC.psp     LMAX=D LOC=S ECUT=70 Ry
  Cu     LDA MT SEMI (Kohlmeyer)          Cu_MT_LDA_SEMI.psp      LMAX=D LOC=S ECUT=80 Ry
  Cu     PW91 MT SEMI (Kohlmeyer)         Cu_MT_PW91_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry
  Cu     BP MT SEMI (Kohlmeyer)           Cu_MT_BP_SEMI.psp       LMAX=D LOC=S ECUT=80 Ry
  Cu     PBE MT SEMI (Kohlmeyer)          Cu_MT_PBE_SEMI.psp      LMAX=D LOC=S ECUT=80 Ry
  Cu     PBE MT SEMI (MPI-Polymerforsch.) Cu_MT_PBE_SEMI_2.08.psp LMAX=D LOC=S ECUT=80 Ry    [51]
  Cu     revPBE MT SEMI (Kohlmeyer)       Cu_MT_revPBE_SEMI.psp   LMAX=D LOC=S ECUT=80 Ry
  Cu     BLYP MT SEMI (Kohlmeyer)         Cu_MT_BLYP_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry    [43]
  Cu     HCTH MT SEMI (Kohlmeyer)         Cu_MT_HCTH_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry    [43]
  Cu     PBE GTH (Goedecker-Rousseau)     Cu_GTH_PBE.psp          LMAX=D LOC=S ECUT=80 Ry
  Cu     BLYP GTH (Goedecker-Rousseau)    Cu_GTH_BLYP.psp         LMAX=D LOC=S ECUT=80 Ry
  Zn     LDA SGS                          Zn_SGS_LDA.psp          LMAX=D LOC=S ECUT=70 Ry
  Zn     LDA MT SEMI (Kohlmeyer)          Zn_MT_LDA_SEMI.psp      LMAX=D LOC=S ECUT=80 Ry
  Zn     BP MT SEMI (Kohlmeyer)           Zn_MT_BP_SEMI.psp       LMAX=D LOC=S ECUT=80 Ry
  Zn     PW91 MT SEMI (Kohlmeyer)         Zn_MT_PW91_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry
  Zn     PBE MT SEMI (Kohlmeyer)          Zn_MT_PBE_SEMI.psp      LMAX=D LOC=S ECUT=80 Ry
  Zn     revPBE MT SEMI (Kohlmeyer)       Zn_MT_revPBE_SEMI.psp   LMAX=D LOC=S ECUT=80 Ry
  Zn     BLYP MT SEMI (Kohlmeyer)         Zn_MT_BLYP_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry    [43]
  Zn     HCTH MT SEMI (Kohlmeyer)         Zn_MT_HCTH_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry    [43]
  Zn     PBE GTH (Krack-Ikeda-Boero)      Zn-q12_GTH_PBE.psp      LMAX=D LOC=D ECUT=90 Ry
  Ga     LDA SGS                          Ga_SGS_LDA.psp          LMAX=D LOC=S ECUT=40 Ry
  Ga     BP MT NLCC (Boero)               Ga_MT_BP_NLCC.psp       LMAX=D LOC=S ECUT=40 Ry
  Ga     BLYP MT (Giannozzi)              Ga_MT_GIA_BLYP.psp      LMAX=D LOC=S ECUT=40 Ry    [35]
  Ga     BLYP MT NLCC (Giannozzi)         Ga_MT_GIA_BLYP_NLCC.psp LMAX=D LOC=S ECUT=40 Ry    [35]
  Ga     LDA GTH (Goedecker)              Ga_GTH_LDA.psp          LMAX=D LOC=P (or D) ECUT=50 Ry
  Ga     PBE GTH (Krack)                  Ga_GTH_PBE.psp          LMAX=D LOC=P (or D) ECUT=50 Ry
  Ga     BLYP GTH (Krack)                 Ga_GTH_BLYP.psp         LMAX=D LOC=P (or D) ECUT=50 Ry
  Ge     LDA SGS                          Ge_SGS_LDA.psp          LMAX=D LOC=D ECUT=20 Ry
  Ge     PW CVB (Pasquarello-DalCorso)    Ge_CVB_PW.psp           LMAX=D LOC=D ECUT=20 Ry    [44]
  Ge     PBE MT (Boero-Oshiyama)          Ge_MT_PBE.psp           LMAX=P LOC=P ECUT=20 Ry
  Ge     PBE MT NLCC (Boero-Oshiyama)     Ge_MT_PBE_NLCC.psp      LMAX=D LOC=D ECUT=20 Ry
  Ge     PBE MT (Boero-Bouzid)            Ge_MT_PBEd.psp          LMAX=D LOC=D ECUT=40 Ry
  Ge     BLYP MT (Vuillumier-Massobrio)   Ge-MT-BLYP.psp          LMAX=P LOC=P ECUT=20 Ry    [49]
  Ge     BLYP MT (Boero-Bouzid)           Ge_MT_BLYPd.psp         LMAX=D LOC=D ECUT=40 Ry
  Ge     PBE GTH (Goedecker)              Ge_GTH_PBE.psp          LMAX=D LOC=D ECUT=40 Ry
  Ge     BLYP GTH (Krack)                 Ge_GTH_BLYP.psp         LMAX=D LOC=D ECUT=40 Ry
  As     LDA SGS                          As_SGS_LDA.psp          LMAX=D LOC=S ECUT=35 Ry    [54]
  As     BLYP MT (Giannozzi)              As_MT_GIA_BLYP.psp      LMAX=D LOC=S ECUT=35 Ry    [35]
  As     PBE MT (Boero-Massobrio)         As_MT_PBE.psp           LMAX=D LOC=D ECUT=35 Ry
  As     PBE GTH (Krack)                  As_GTH_PBE.psp          LMAX=D LOC=D ECUT=40 Ry    [54]
  As     BLYP GTH (Krack)                 As_GTH_BLYP.psp         LMAX=D LOC=D ECUT=40 Ry    [54]
  Se     LDA SGS                          Se_SGS_LDA.psp          LMAX=D LOC=D ECUT=20 Ry    [29]
  Se     PW CVB (Pasquarello-DalCorso)    Se_CVB_PW.psp           LMAX=D LOC=D ECUT=20 Ry    [44]
  Se     LDA MT (Boero)                   Se_MT_LDA.psp           LMAX=D LOC=D ECUT=20 Ry
  Se     OBE MT (Boero-Bouzid)            Se_MT_PBE.psp           LMAX=D LOC=D ECUT=20 Ry
  Se     BLYP MT (Boero)                  Se_MT_BLYP.psp          LMAX=D LOC=D ECUT=20 Ry
  Se     BLYP MT (Vuillumier-Massobrio)   Se_MT_BLYP2.psp         LMAX=P LOC=P ECUT=20 Ry    [49]
  Se     HCTH MT (Boero)                  Se_MT_HCTH.psp          LMAX=D LOC=D ECUT=20 Ry
  Se     PBE GTH (Goedecker)              Se_GTH_PBE.psp          LMAX=D LOC=D ECUT=20 Ry
  Se     BLYP GTH (Boero-Ikeda)           Se-q6_GTH_BLYP.psp      LMAX=D LOC=D ECUT=20 Ry
  Br     LDA SGS                          Br_SGS_LDA.psp          LMAX=P LOC=P ECUT=70 Ry
  Br     BLYP MT (Sprik-Ikeda)            Br_MT_BLYP.psp          LMAX=D LOC=D ECUT=70 Ry    [27]
  Br     PBE MT (Ikeda)                   Br_MT_PBE.psp           LMAX=D LOC=D ECUT=70 Ry    [27]
  Br     revPBE MT (Ikeda)                Br_MT_revPBE.psp        LMAX=D LOC=D ECUT=70 Ry
  Br     HCTH MT (Boero-Ikeda)            Br_MT_HCTH.psp          LMAX=D LOC=D ECUT=70 Ry
  Br     OLYP MT (Boero-Ikeda)            Br_MT_OLYP.psp          LMAX=D LOC=D ECUT=70 Ry
  Br     XLYP MT (Boero-Ikeda)            Br_MT_XLYP.psp          LMAX=D LOC=D ECUT=70 Ry
  Br     BLYP GTH (Krack)                 Br_GTH_BLYP.psp         LMAX=D LOC=D ECUT=70 Ry
  Rb     PBE GTH SEMI (Ikeda)             Rb_GTH_PBE_SEMI.psp     LMAX=D LOC=D ECUT=80 Ry    [55]
  Rb     BLYP GTH SEMI (Ikeda)            Rb_GTH_BLYP_SEMI.psp    LMAX=D LOC=D ECUT=80 Ry    [55]
  Rb     HCTH GTH SEMI (Ikeda)            Rb_GTH_HCTH_SEMI.psp    LMAX=D LOC=D ECUT=80 Ry    [55]
  Y      PBE MT NLCC (Boero-Oshikiri)     Y_MT_PBE_NLCC.psp       LMAX=D LOC=S SKIP=P ECUT=70 Ry [57]
  Y      BLYP MT NLCC (Boero-Oshikiri)    Y_MT_BLYP_NLCC.psp      LMAX=D LOC=S SKIP=P ECUT=70 Ry [56]
  Y      BLYP MT SEMI (Boero-Oshikiri)    Y_MT_BLYP_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry    [56]
  Y      HCTH MT SEMI (Boero-Ikeda)       Y_MT_HCTH_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry    [32]
  Y      PBE MT SEMI (Boero)              Y_MT_PBE_SEMI.psp       LMAX=D LOC=D ECUT=80 Ry
  Y      PW91 MT SEMI (Boero)             Y_MT_PW91_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry
  Y      XLYP MT SEMI (Boero)             Y_MT_XLYP_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry
  Zr     BLYP SEMI (Giannozzi)            Zr_SEMI_GIA.psp         LMAX=D LOC=D ECUT=70 Ry    [26]
  Zr     BLYP SEMI (Boero-Giannozzi)      Zr_SEMI_BLYP.psp        LMAX=D LOC=D ECUT=70 Ry
  Zr     PBE SEMI (Boero)                 Zr_MT_SEMI_PBE.psp      LMAX=D LOC=D ECUT=70 Ry
  Zr     HCTH SEMI (Boero-Ikeda)          Zr_MT_HCTH_SEMI.psp     LMAX=D LOC=D ECUT=70 Ry
  Zr     PBE USPP-Vanderbilt (Boero)      040-Zr-gpbe-bm.uspp     LMAX=D LOC=D ECUT=35 Ry
  Mo     BP MT SEMI (Hutter)              Mo_MT_BP_SEMI.psp       LMAX=D LOC=D ECUT=70 Ry
  Mo     PBE MT SEMI (Boero)              Mo_MT_PBE_SEMI.psp      LMAX=D LOC=D ECUT=70 Ry
  Mo     BLYP MT SEMI (Boero)             Mo_MT_BLYP_SEMI.psp     LMAX=D LOC=D ECUT=70 Ry
  Mo     HCTH MT SEMI (Boero)             Mo_MT_HCTH_SEMI.psp     LMAX=D LOC=D ECUT=70 Ry
  Mo     PBE GTH (Goedecker-Rousseau)     Mo_GTH_PBE.psp          LMAX=D LOC=D ECUT=90 Ry
  Mo     BLYP GTH (Boero-Ikeda))          Mo-q14_GTH_BLYP.psp     LMAX=D LOC=D ECUT=90 Ry
  Rh     BLYP MT NLCC (Boero-Pichierri)   Rh_MT_BLYP_NLCC.psp     LMAX=D LOC=S ECUT=70 Ry
  Rh     BLYP MT SEMI (Boero-Pichierri)   Rh_MT_BLYP_SEMI.psp     LMAX=D LOC=D ECUT=90 Ry
  Rh     PBE MT NLCC (Boero-Pichierri)    Rh_MT_PBE_NLCC.psp      LMAX=D LOC=S ECUT=70 Ry
  Rh     HCTH MT NLCC (Boero-Pichierri)   Rh_MT_HCTH_NLCC.psp     LMAX=D LOC=S ECUT=70 Ry
  Rh     OLYP MT NLCC (Boero-Pichierri)   Rh_MT_OLYP_NLCC.psp     LMAX=D LOC=S ECUT=70 Ry
  Pd     BLYP MT NLCC (Boero-Ikeda)       Pd_MT_BLYP_NLCC.psp     LMAX=D LOC=S ECUT=100 Ry   [46]
  Pd     PBE GTH SEMI (Krack)             Pd_GTH_PBE.psp          LMAX=D LOC=D ECUT=80 Ry    [54]
  Pd     BLYP GTH SEMI (Krack)            Pd_GTH_BLYP.psp         LMAX=D LOC=D ECUT=80 Ry    [54]
  Ag     BLYP MT SEMI (Pagliai)           Ag_SEMI_BLYP.psp        LMAX=D LOC=D ECUT=80 Ry    [53]
  Cd     LDA SGS                          Cd_SGS_LDA.psp          LMAX=D LOC=S ECUT=50 Ry    [28]
  Cd     LDA HSC NLCC (Dal Corso)         Cd_HSC_LDA_NLCC.psp     LMAX=D LOC=S ECUT=24 Ry    [28]
  Cd     LDA MT NLCC (Boero)              Cd_MT_LDA_NLCC.psp      LMAX=D LOC=P ECUT=24 Ry
  Cd     BLYP MT NLCC (Boero)             Cd_MT_BLYP_NLCC.psp     LMAX=D LOC=P ECUT=24 Ry
  Cd     HCTH MT NLCC (Boero)             Cd_MT_HCTH_NLCC.psp     LMAX=D LOC=P ECUT=24 Ry
  Cd     LDA CVB (Dal Corso)              Cd_CVB_LDA.psp          LMAX=P LOC=P ECUT=24 Ry    [28]
  Cd     PBE GTH (Krack)                  Cd_GTH_PBE.psp          LMAX=D LOC=D ECUT=90 Ry
  In     LDA SGS                          In_SGS_LDA.psp          LMAX=D LOC=P ECUT=80 Ry
  In     BLYP MT NLCC (Boero-Oshikiri)    In_MT_BLYP_NLCC.psp     LMAX=D LOC=P ECUT=80 Ry    [33]
  In     PBE MT NLCC (Boero-Oshikiri)     In_MT_PBE_NLCC.psp      LMAX=D LOC=P ECUT=80 Ry
  In     BLYP GTH (Boero-Ikeda)           In-q13_GTH_BLYP.psp     LMAX=F LOC=F ECUT=90 Ry
  Sn     BLYP MT NLCC (Boero-Oshikiri)    Sn_MT_BLYP_NLCC.psp     LMAX=D LOC=P ECUT=80 Ry
  Sb     LDA SGS                          Sb_SGS_LDA.psp          LMAX=P LOC=P ECUT=50 Ry
  Sb     PBE GTH (Krack)                  Sb_GTH_PBE.psp          LMAX=D LOC=S ECUT=40 Ry
  Sb     PBE MT (Boero-Bouzid)            Sb_MT_PBE.psp           LMAX=D LOC=P ECUT=40 Ry
  Sb     BLYP MT (Boero-Massobrio)        Sb_MT_BLYP.psp          LMAX=D LOC=P ECUT=40 Ry
  Sb     HCTH MT (Boero-Massobrio)        Sb_MT_HCTH.psp          LMAX=D LOC=P ECUT=40 Ry
  Te     LDA SGS                          Te_SGS_LDA.psp          LMAX=D LOC=P ECUT=24 Ry    [28]
  Te     PBE MT (Akola-Jones)             Te_MT_PBE.psp           LMAX=D LOC=D ECUT=40 Ry    [50]
  Te     PBESol MT (Akola-Jones)          Te_MT_PBESol.psp        LMAX=D LOC=D ECUT=40 Ry    [50]
  Te     BLYP MT (Boero-Micoulaut)        Te_MT_BLYP.psp          LMAX=D LOC=P ECUT=40 Ry
  Te     HCTH MT (Boero-Micoulaut)        Te_MT_HCTH.psp          LMAX=D LOC=P ECUT=40 Ry
  Te     BLYP GTH (Boero-Krack)           Te_GTH_BLYP.psp         LMAX=D LOC=D ECUT=40 Ry
  I      LDA SGS                          I_SGS_LDA.psp           LMAX=D LOC=P ECUT=35 Ry
  I      PBE MT (Boero)                   I_MT_PBE.psp            LMAX=P LOC=P ECUT=50 Ry
  I      BLYP MT (Boero)                  I_MT_BLYP.psp           LMAX=P LOC=P ECUT=50 Ry
  I      PBE GTH (Ikeda-Boero)            I_GTH_PBE.psp           LMAX=D LOC=D ECUT=50 Ry
  I      BLYP GTH (Ikeda-Boero)           I_GTH_BLYP.psp          LMAX=D LOC=D ECUT=50 Ry
  Xe     LDA SGS                          Xe_SGS_LDA.psp          LMAX=D LOC=P ECUT=35 Ry
  Cs     BLYP MT (Giannozzi)              Cs_MT_GIA_BLYP_NLCC.psp LMAX=D LOC=P ECUT=50 Ry     [8]
  Cs     BLYP MT SEMI (Giannozzi)         Cs_MT_GIA_BLYP_SEMI.psp LMAX=D LOC=S ECUT=80 Ry     [8]
  Cs     PBE GTH (Ikeda-Krack)            Cs_GTH_PBE_SEMI.psp     LMAX=F LOC=S ECUT=80 Ry    [55]
  Cs     revPBE GTH (Ikeda)               Cs_GTH_revPBE_SEMI.psp  LMAX=D LOC=S ECUT=80 Ry
  Cs     BLYP GTH (Ikeda)                 Cs_GTH_BLYP_SEMI.psp    LMAX=D LOC=S ECUT=80 Ry    [55]
  Cs     HCTH GTH (Krack-Ikeda)           Cs_GTH_HCTH_SEMI.psp    LMAX=D LOC=S ECUT=80 Ry    [55]
  Ba     BLYP MT NLCC (Boero)             Ba_MT_BLYP_NLCC.psp     LMAX=P LOC=S ECUT=50 Ry
  Ba     BLYP MT SEMI (Boero)             Ba_MT_BLYP_SEMI.psp     LMAX=P LOC=P ECUT=80 Ry
  La     PBE MT SEMI (Ikeda-Boero)        La_MT_PBE_SEMI.psp      LMAX=F LOC=D ECUT=90 Ry
  La     BLYP MT SEMI (Ikeda-Boero)       La_MT_BLYP_SEMI.psp     LMAX=F LOC=D ECUT=90 Ry
  La     HCTH MT SEMI (Ikeda-Boero)       La_MT_HCTH_SEMI.psp     LMAX=F LOC=D ECUT=90 Ry    [32]
  La     PW91 MT SEMI (Boero)             La_MT_PW91_SEMI.psp     LMAX=F LOC=D ECUT=90 Ry
  La     XLYP MT SEMI (Boero)             La_MT_PW91_SEMI.psp     LMAX=F LOC=D ECUT=90 Ry
  La     PBE USPP-Vanderbilt (Ikeda)      057-La-gpbe-ike.uspp    LMAX=D LOC=D ECUT=50 Ry
  Ce     PBE GTH (Boero-Ikeda)            Ce-q12_GTH_PBE.psp      LMAX=F LOC=S ECUT=80 Ry
  Ce     BLYP GTH (Boero-Ikeda)           Ce-q12_GTH_BLYP.psp     LMAX=F LOC=S ECUT=80 Ry
  Ce     HCTH GTH (Boero-Ikeda)           Ce-q12_GTH_HCTH.psp     LMAX=F LOC=S ECUT=80 Ry
  Gd     PBE GTH Ikeda-Boero)             Gd_GTH_PBE.psp          LMAX=F LOC=S ECUT=80 Ry
  Gd     BLYP GTH (Ikeda-Boero)           Gd_GTH_BLYP.psp         LMAX=F LOC=S ECUT=80 Ry
  Tb     BLYP GTH (Ikeda-Boero)           Tb_BLYP_GTH.psp         LMAX=F LOC=S ECUT=80 Ry
  Hf     PBE MT (Boero-Shiraishi)         Hf_MT_PBE.psp           LMAX=D LOC=S ECUT=70 Ry    [37]
  Hf     BLYP MT (Boero-Shiraishi)        Hf_MT_BLYP.psp          LMAX=D LOC=S ECUT=70 Ry
  Hf     OLYP MT (Boero-Shiraishi)        Hf_MT_OLYP.psp          LMAX=D LOC=S ECUT=70 Ry
  Hf     HCTH MT (Boero)                  Hf_MT_HCTH.psp          LMAX=D LOC=S ECUT=70 Ry
  Hf     XLYP MT (Boero)                  Hf_MT_XLYP.psp          LMAX=D LOC=S ECUT=70 Ry
  Ta     BLYP MT (Boero-Ramaniah)         Ta_MT_BLYP.psp          LMAX=D LOC=S ECUT=40 Ry    [30]
  W      LDA BHS (Baroni-Bungaro)         W_BHS_LDA.psp           LMAX=D LOC=P ECUT=28 Ry    [31]
  W      BLYP MT NLCC (Oshikiri)          W_MT_BLYP_NLCC.psp      LMAX=D LOC=S ECUT=70 Ry
  W      BLYP GTH (Boero-Ikeda)           W-q6-GTH_BLYP.psp       LMAX=D LOC=D ECUT=90 Ry
  W      BLYP GTH (Boero-Ikeda)           W-q14-GTH_BLYP.psp      LMAX=D LOC=D ECUT=90 Ry
  Re     PBE GTH q7                       Re-q7_GTH_PBE.psp       LMAX=D LOC=D ECUT=90 Ry
  Re     PBE GTH q15                      Re-q15_GTH_PBE.psp      LMAX=D LOC=D ECUT=90 Ry
  Re     BLYP GTH q7                      Re-q7_GTH_PBE.psp       LMAX=D LOC=D ECUT=90 Ry
  Re     BLYP GTH q15                     Re-q15_GTH_PBE.psp      LMAX=D LOC=D ECUT=90 Ry
  Pt     BP MT SEMI (Giannozzi)           Pt_MT_GIA_BP_SEMI.psp   LMAX=D LOC=D ECUT=80 Ry    [47]
  Pt     BLYP MT SEMI (Giannozzi)         Pt_MT_GIA_BLYP_SEMI.psp LMAX=D LOC=D ECUT=80 Ry    [48]
  Pt     PBE MT SEMI (Boero)              Pt_MT_PBE_SEMI.psp      LMAX=D LOC=D ECUT=80 Ry
  Pt     HCTH MT SEMI (Boero)             Pt_MT_HCTH_SEMI.psp     LMAX=D LOC=D ECUT=80 Ry
  Pt     PBE GTH SEMI (Krack)             Pt_GTH_PBE.psp          LMAX=D LOC=D ECUT=80 Ry
  Au     BP MT NLCC (Rousseau)            Au_MT_BP_NLCC.psp       LMAX=D LOC=P ECUT=90 Ry
  Au     BLYP MT NLCC (Boero-Rojas)       Au_MT_BLYP_NLCC.psp     LMAX=D LOC=P ECUT=90 Ry
  Au     LDA GTH (Goedecker-Koizumi)      Au_GTH_LDA.psp          LMAX=D LOC=P ECUT=90 Ry     [6]
  Au     BP GTH (Goedecker)               Au_GTH_BP.psp           LMAX=F LOC=F ECUT=90 Ry     [6]
  Au     PBE GTH (Goedecker)              Au_GTH_PBE.psp          LMAX=F LOC=F ECUT=90 Ry
  Au     PBE GTH (Rousseau)               Au_GTH_PBE-new.psp      LMAX=F LOC=F ECUT=90 Ry
  Au     BLYP GTH (Goedecker)             Au_GTH_BLYP.psp         LMAX=D LOC=P ECUT=90 Ry
  Au     PBE-q11 GTH (Ikeda-Koizumi)      Au-q11_GTH_PBE.psp      LMAX=D LOC=P ECUT=90 Ry
  Au     PBE-q19 GTH (Ikeda)              Au-q19_GTH_PBE.psp      LMAX=D LOC=P ECUT=90 Ry
  Au     BLYP-q11 (Ikeda-Boero-Koizumi)   Au-q11_GTH_BLYP.psp     LMAX=D LOC=P ECUT=90 Ry
  Au     BLYP-q19 (Ikeda-Boero-Koizumi)   Au-q19_GTH_BLYP.psp     LMAX=D LOC=P ECUT=90 Ry
  Au     PBE USPP-Vanderbilt (Ikeda-Boero)Au_VDB_PBE.psp          LMAX=F LOC=F ECUT=30 Ry
  Hg     LDA SEMI (Boero-Gygi)            Hg_MT_LDA_SEMI.psp      LMAX=D LOC=S ECUT=80 Ry    [52]
  Hg     PBE SEMI (Boero-Gygi)            Hg_MT_PBE_SEMI.psp      LMAX=D LOC=S ECUT=80 Ry    [52]
  Hg     BLYP SEMI (Boero-Gygi)           Hg_MT_BLYP_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry    [52]
  Hg     BLYP SEMI (Boero-Gygi)           Hg_MT_HCTH_SEMI.psp     LMAX=D LOC=S ECUT=80 Ry    [52]
  Pb     PBE MT NLCC (Boero-Ikeda)        Pb_MT_PBE_NLCC.psp      LMAX=P LOC=P ECUT=80 Ry    [45]
  Pb     BLYP MT NLCC (Boero-Ikeda)       Pb_MT_BLYP_NLCC.psp     LMAX=P LOC=P ECUT=80 Ry
  Pb     HCTH MT NLCC (Boero-Ikeda)       Pb_MT_HCTH_NLCC.psp     LMAX=P LOC=P ECUT=80 Ry
  Pb     BLYP MT SEMI (Boero-Andreoni)    Pb_MT_BLYP_SEMI.psp     LMAX=D LOC=D ECUT=90 Ry
  Pb     PBE GTH (Boero-Ikeda)            Pb_GTH_PBE.psp          LMAX=D LOC=D ECUT=90 Ry
  Th     PBE GTH (Boero-Ikeda)            Th_GTH_PBE.psp          LMAX=F LOC=S ECUT=100 Ry
  U      BP GTH (Rousseau)                U_GTH_BP.psp            LMAX=F LOC=S ECUT=100 Ry
  U      PBE GTH (Rousseau)               U_GTH_PBE.psp           LMAX=F LOC=S ECUT=100 Ry
  U      BLYP GTH (Rousseau)              U_GTH_BLYP.psp          LMAX=F LOC=S ECUT=100 Ry
  Pu     PBE GTH (Rousseau)               Pu_GTH_PBE.psp          LMAX=F LOC=S ECUT=120 Ry
  Cm     HCTH GTH (Boero-Rousseau)        Cm_GTH_HCTH.psp         LMAX=F LOC=S ECUT=120 Ry
_______________________________________________________________________
 SPECIAL PESUDOPOTENTIALS: these are pseudopotentials constructed
 with 1/2 hole in the 1s state and are intended to be used with
 the X-ray spectra routine of CPMD (see CPMD manual for details):

 B       GGA MT (Boero)                   B_MT_GGA_HOLE.psp
 B       PBE MT (Boero)                   B_MT_PBE_HOLE.psp
 B       revPBE MT (Boero)                B_MT_revPBE_HOLE.psp
 B       BLYP MT (Boero)                  B_MT_BLYP_HOLE.psp
 B       OLYP MT (Boero)                  B_MT_OLYP_HOLE.psp
 B       HCTH MT (Boero)                  B_MT_HCTH_HOLE.psp
 B       XLYP MT (Boero)                  B_MT_XLYP_HOLE.psp
 C       GGA MT (Boero)                   C_MT_GGA_HOLE.psp
 C       PBE MT (Boero)                   C_MT_PBE_HOLE.psp
 C       revPBE MT (Boero)                C_MT_revPBE_HOLE.psp
 C       BLYP MT (Boero)                  C_MT_BLYP_HOLE.psp
 C       OLYP MT (Boero)                  C_MT_OLYP_HOLE.psp
 C       HCTH MT (Boero)                  C_MT_HCTH_HOLE.psp
 C       XLYP MT (Boero)                  C_MT_XLYP_HOLE.psp
 N       GGA MT (Boero)                   N_MT_GGA_HOLE.psp
 N       PBE MT (Boero)                   N_MT_PBE_HOLE.psp
 N       revPBE MT (Boero)                N_MT_revPBE_HOLE.psp
 N       BLYP MT (Boero)                  N_MT_BLYP_HOLE.psp
 N       OLYP MT (Boero)                  N_MT_OLYP_HOLE.psp
 N       HCTH MT (Boero)                  N_MT_HCTH_HOLE.psp
 N       XLYP MT (Boero)                  N_MT_XLYP_HOLE.psp
 O       GGA MT (Boero)                   O_MT_GGA_HOLE.psp
 O       PBE MT (Boero)                   O_MT_PBE_HOLE.psp
 O       revPBE MT (Boero)                O_MT_revPBE_HOLE.psp
 O       BLYP MT (Boero)                  O_MT_BLYP_HOLE.psp
 O       OLYP MT (Boero)                  O_MT_OLYP_HOLE.psp
 O       HCTH MT (Ikeda)                  O_MT_HCTH_HOLE.psp
 O       XLYP MT (Boero)                  O_MT_XLYP_HOLE.psp
 F       PBE MT (Boero)                   F_MT_PBE_HOLE.psp
 F       BLYP MT (Boero)                  F_MT_BLYP_HOLE.psp
 F       HCTH MT (Boero)                  F_MT_HCTH_HOLE.psp
 Si      GGA MT (Boero)                   Si_MT_GGA_HOLE.psp
 Si      PBE MT (Boero)                   Si_MT_PBE_HOLE.psp
 Si      HCTH MT (Boero)                  Si_MT_HCTH_HOLE.psp
 Si      XLYP MT (Boero)                  Si_MT_XLYP_HOLE.psp
_______________________________________________________________________
 Optimized effective core potential for QM/MM linking:

 C       OECP BLYP (Tavernelli)           C_GIA_DUM_AN_BLYP.oecp
 C       OECP PBE (Boero-Reich)           C_GIA_DUM_AN_PBE.oecp
 C       OECP HCTH (Boero-Reich)          C_GIA_DUM_AN_HCTH.oecp
 C       OECP PBE positive (Boero-Reich)  CP_GIA_DUM_AN_PBE.oecp
 C       OECP PBE pos. s-p (Boero-Reich)  CPS_GIA_DUM_AN_PBE.oecp
 C       OECP PBE negative (Boero-Reich)  CM_GIA_DUM_AN_PBE.oecp
 Note: These pseudopotentials are intended only for valence
       saturation on C sp3 bond cutting in hybrid QM/MM.
       The type and charge of the OECP must be carefully
       selected according to the partial charge of the C
       atom on which the cut is performed.
_______________________________________________________________________
 List of the short-hand notations used to identify the
 type of pseudopotential/functional and related references:
 LDA    = Local Density Approximation. J.P. Perdew and
          A. Zunger, Phys. Rev. B 23, 5048 (1981).
 BP     = Becke-Perdew Gradient Corrected. A.D. Becke,
          Phys. Rev. A 38, 3098 (1988); J.P. Perdew,
          Phys. Rev. B 33, 8822 (1986).
 PW91   = Perdew-Wang. J.P. Perdew and Y. Wang, Phys. Rev. B
          45, 13244 (1992)
 GGA    = Generalized Gradient Approximation. J.P. Perdew,
          J.A. Chevary,  S.H. Vosko, K.A. Jackson, M.R. Pederson,
          D.J. Singh and C. Fiolhais, Phys. Rev. B 46, 6671 (1992).
 BLYP   = Becke-Lee-Yang-Parr Gradient Corrected. A.D. Becke,
          Phys. Rev. A 38, 3098 (1988); C. Lee, W. Yang
          and R.G. Parr, Phys. Rev. B 37, 785 (1988).
 PBE    = Perdew-Burke-Ernzerhof Gradient Corrected.
          J.P. Perdew, K. Burke and M. Ernzerhof,
          Phys. Rev. Lett. 77, 3865 (1996).
 revPBE = revised PBE. Y. Zhang and W. Yang, Phys. Rev.
          Lett. 80, 890 (1998).
 HCTH   = Hamprecht-Cohen-Tozer-Handy. F.A. Hamprecht,
          A.J. Cohen, D.J. Tozer and N.C. Handy, J. Chem.
          Phys. 109, 6264 (1998).
 OLYP   = OPTX of Handy + LYP. N.C. Handy and A.J. Cohen,
          J. Chem. Phys. 116, 5411 (2002).
 XLYP   = Exchange=(0.722 B88 + 0.347 PW91), correlation=LYP.
          X. Xu and W.A. Goddard III, Proc. Nat. Ac. Sci. 101,
          2673 (2004).
 BHS    = Bachelet-Hamann-Schlueter. G. B. Bachelet, D. R.
          Hamann and M. Schluter, Phys. Rev. B 26, 4199 (1982).
 SGS    = Stumpf-Gonze-Schaeffler. X. Gonze, R. Stumpf, and
          M. Scheffler, Phys. Rev. B 44, 8503 (1991)
 HSC    = Hamann-Schlueter-Chang. D. R. Hamann, M. Schluter,
          and C. Chiang, Phys. Rev. Lett. 43, 1494 (1979).
 MT     = Martins-Trouiller. N. Troullier and J. L. Martins,
          Phys. Rev. B 43, 1993 (1991).
 CVB    = Von Barth-Car. U. von Barth and R. Car (unpublished)
 GTH    = Goedecker-type. S. Goedecker, M. Teter, and J. Hutter
          Phys. Rev. B 54, 1703 (1996).
          C. Hartwigsen, S. Goedecker, and J. Hutter,
          Phys. Rev. B 58, 3641 (1998)
          M. Krack, Theor. Chem. Acc. 114, 145 (2005)
 NLCC   = Non-Linear Core Corrections. S. G. Louie, F. Froyen
          and M. L. Cohen, Phys. Rev. B 26, 1738 (1982).
 SEMI   = Semicore States included
 uspp   = New Vanderbilt Ultrasoft pseudopotential
          (WARNING: binary files only ! If they do not
           work on your machine, you have to regenerate
           them using the uspp code and related input files)

 In ( ) is indicated the person who has generated the
 pseudopotential ...if known.

________________________________________________________________
 Known Original References (KOR), i.e.  where the above listed
 pseudopotentials have been used for the first time. Several
 pseudopotentials have been used in many more publications not
 listed here for space reasons and some of them have been either
 tested but not used in published papers or tested and used in
 unpublished works.
 This is the case of e.g. the extensively used analytical
 Car-von Barth Hydrogen originally built by P. Giannozzi.
 PLEASE NOTE THAT DUE TO THE DIFFICULTY IN TRACING BACK THE
 ORIGINAL CONSTRUCTION AND FIRST USE OF SEVERAL PSEUDOPOTENTIALS,
 MANY REFERENCES ARE STILL MISSING OR INCORRECTLY CITED.
 YOU ARE KINDLY ASKED TO NOTIFY US ERRORS AND OMISSISONS.

 KOR List:
 [1] X. Gonze, R. Stumpf, M. Scheffler,
     Phys. Rev. B 44, 8503 (1991).
     G.B. Bachelet, D.R. Hamann, M. Schlüter,
     Phys. Rev. B 26, 4199 (1982).
 [2] O. Pfaffenzeller, D. Hohl, P. Ballone
     Phys. Rev. Lett. 74, 2599 (1995).
 [3] M. Boero, M. Parrinello, K. Terakura
     J. Am. Chem. Soc. 120, 2746 (1998).
 [4] R. Rousseau, M. Boero, M. Bernasconi, M. Parrinello, K. Terakura
     Phys. Rev. Lett. 83, 2218 (1999).
 [5] M. Boero, K. Terakura, M. Tateno
     J. Am. Chem. Soc. 124, 8949 (2002).
 [6] S. Goedecker, M. Teter, J. Hutter
     Phys. Rev. B 54, 1703 (1996).
 [7] M. Sprik, J. Hutter, M. Parrinello
     J. Chem. Phys. 105, 1142 (1996).
 [8] W. Andreoni, P. Giannozzi, J.F. Armbruster, M. Knupfer, J. Fink
     Europhys. Lett. 34, 699 (1996).
 [9] R. Rousseau, D. Marx
     Chem. Eur. J. 6, 2982 (2000).
[10] M. Oshikiri, F. Aryasetiawan, M. Boero
     Mat. Res. Soc. Symp. Proc. 654, AA5.10.1 (2001).
[11] W. Andreoni, A. Curioni, M. Boero,
     European Phys. Soc. 10th General Conference - Symposium
     on Fullerenes, Sevilla (Spain) 1996.
[12] F. Favot, A. Dal Corso,
     Phys. Rev. B 60, 11427 (1999).
[13] W. Andreoni, D. Scharf, P. Giannozzi,
     Chem. Phys. Lett. 173, 449 (1990).
[14] A. Simunek, J. Vackár, K. Kunc, J. Hutter,
     Eur. Phys. J. B 14, 245 (2000).
[15] M. Boero, W. Andreoni,
     Chem. Phys. Lett. 265, 24 (1997).
[16] R. Car, M. Parrinello,
     Phys. Rev. Lett. 55, 2471 (1985).
[17] J. Sarnthein, A. Pasquarello, R. Car,
     Phys. Rev. Lett. 74, 4682 (1995).
[18] A. Pasquarello,
     Appl. Surf. Sci. 166, 451 (2000).
[19] D. Donadio, M. Bernasconi, M. Boero,
     Phys. Rev. Lett. 87, 195504 (2001).
[20] N. L. Doltsinis, M. Spirk,
     Phys. Chem. Chem. Phys. 5, 2612 (2003).
[21] M. Boero, K. Terakura, M. Parrinello,
     Int. J. Mol. Sci. 3, 395 (2002).
[22] C. Rovira, M. Parrinello
     Int. J. Quantum Chem. 70, 387 (1998)
[23] I. M. L. Billas, C. Massobrio, M. Boero, T. P. Martin,
     Comput. Mat. Sci. 17,  191 (2000).
[24] L. M. Ramaniah, M. Bernasconi, M. Parrinello,
     J. Chem. Phys. 109, 6839 (1998).
[25] L. M. Ramaniah, M. Bernasconi, M. Parrinello,
     J. Chem. Phys. 111, 1587 (1999).
[26] G. Stapper, M. Bernasconi, N. Nicoloso, M. Parrinello,
     Phys. Rev. B 59, 797 (1999).
[27] T. Ikeda, M. Sprik, K. Terakura, M. Parrinello,
     J. Chem. Phys. 111, 1595 (1999).
[28] A. Dal Corso, R. Resta, S. Baroni,
     Phys. Rev. B 47, 16252 (1993).
[29] A. Dal Corso and R. Resta,
     Phys. Rev. B 50, 4327 (1994).
[30] L. M. Ramaniah, M. Boero, M. Laghate,
     Phys. Rev. B 70, 035411 (2004).
[31] C. Bungaro, S. de Gironcoli S, S. Baroni,
     Phys. Rev.Lett. 77, 2491 (1996).
[32] T. Ikeda, M. Hirata, T. Kimura,
     J. Chem. Phys. 122, 024510 (2005).
[33] M. Oshikiri, M. Boero, J. Ye, Z. Zou, G. Kido,
     J. Chem. Phys. 117, 7313 (2002).
[34] N. Troullier, J. L. Martins,
     Phys. Rev. B 43, 1993 (1991).
[35] A. A. Bonapasta, M. Capizzi, P. Giannozzi,
     Phys. Rev. B 57, 12923 (1998).
[36] V. Brazdova, M.V. Granduglia-Pirovano, J. Sauer,
     Phys. Rev. B 69, 165420 (2004).
[37] N. Umezawa, K. Shiraishi, T. Ohno, M. Boero, H. Watanabe,
     T. Chikyow, K. Torii, K. Yamabe, K. Yamada, Y. Nara
     Physica B 376-377, 392 (2006).
[38] F. L. Gervasio, M. Boero, M. Parrinello,
     Angew. Chem. Int. Ed. 45, 5606 (2006).
[39] C. Rovira, M. Parrinello,
     Biophys. J. 78, 93 (2000).
[40] M. Boero, T. Ikeda, E. Ito, K. Terakura,
     J. Am. Chem. Soc. 128, 16798 (2006).
[41] T. Ikeda, M. Boero, K. Terakura,
     J. Chem. Phys. 126, 034501 (2007).
[42] C. Rovira, K. Kunc, J. Hutter, M. Parrinello,
     Inorg. Chem. 40, 11 (2001).
[43] J. Blumberger, I. Tavernelli, M. L. Klein,
     Abstr. Papers Am. Chem. Soc. 230 U2880 234-Phys (2005)
[44] A. DalCorso, A. Pasquarello, A. Baldereschi, R. Car,
     Phys. Rev. B. 53, 1180 (1996)
[45] L. C. Balbas, J. L. Martins,
     Phys. Rev. B 54, 2937 (1996)
[46] F. Aguilera-Granja, J. Ferrer, A. Vega,
     Phys. Rev. B 74, 174416 (2006)
[47] P. Carloni, M. Sprik, W. Andreoni,
     J. Phys. Chem. B 104, 823 (2000)
[48] E.-G. Kim, K. Schmidt, W. R. Caseri, T. Kreouzis,
     N. Stingelin-Stutzmann and J. L. Bredas,
     Adv. Mater. 18, 2039 (2006)
[49] C. Massobrio, A. Pasquarello,
     Phys. Rev. B 77, 144207 (2008)
[50] J. Akola, R. O. Jones, S. Kohara, T. Usuki and E. Bychov,
     Phys. Rev. B 81, 094202 (2010)
[51] L. M. Ghiringhelli,  L. Delle Site,
     J. Am. Chem. Soc. 130, 2634 (2008)
[52] http://fpmd.ucdavis.edu/potentials/Hg/index.htm
[53] M. Pagliai, M. Muniz-Miranda, G. Cardini, V. Schettino
     J. Phys. Chem. A 113, 15198 (2009)
[54] M. Krack, Theor. Chem. Acc. 114, 145 (2005)
[55] T. Ikeda and M. Boero, J. Chem. Phys. 137, 041101 (2012)
[57] M. Oshikiri, J. Ye, M. Boero, J. Phys. Chem. C 118, 8331 (2014)
[58] M. Oshikiri, J. Ye, M. Boero, J. Phys. Chem. C 118, 12845 (2014)
[59] U. Rothlisberger, W. Andreoni, P.Giannozzi, J. Chem. Phys. 96, 1248 (1992)
[60] T. Nakano, Y. Harashima , K. Chokawa, K. Shiraishi, A. Oshiyama,
     Y. Kangawa , S. Usami, N.aMayama, K. Toda, A. Tanaka, Y. Honda, H. Amano,
     Appl. Phys. Lett. 117, 012105 (2020)
[61] M. Boero, K. M. Bui, K. Shiraishi, K. Ishisone, Y. Kangawa, A. Oshiyama,
     Apppl. Surf. Sci. 599, 153935 (2022)
________________________________________________________________
Present update: 15 November 2023
________________________________________________________________
 DISCLAIMER: the present pseudopotential library is supplied
             (freely) "as is". All the pseudopotentials have
             been extensively tested and most of them already
