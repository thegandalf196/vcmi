# New Horizons frontend handoff (W2)

## Live convenience feedback and newly authorized Extras integration — active

SOURCE HOLD RELEASED explicitly by Build. Next authorized rebase delivered as
ONE patch `research/combat-source2-on-50f07708.patch`; git apply --check PASS
against exact50f roots. Only2changed chooser files+2newFocus files; other4client
bodies already equal sealedsource2. Adds showAll refresh to both chooser and Focus
selector, preserving source1 repair while closing selector's same redraw gap.
Current compiled roots/frozen offers untouched; no unpaired Runtime APIs applied.
Build/Content received concrete patch for separate source2 effects/context/reentry
review. Runtime4/CMake/test-enabled64-case pairing and explicit dispatch decision
still required; ENABLE_TEST OFF in previousFULL is not that native test lane.
No B art, new art import, rules edits or GUI. Full scope retained.
NEW narrow Focus text-fit fix: preferred successor
`research/combat-source2-on-50f07708-row32.patch` changes ONLY row text height28->32
versus preserved first rebase patch. CMultiLineLabel::showAll actually clips to
text rectangle; current bitmapSmall lineheight16 means two lines need32, not28.
Y2+height32 ends34 within unchanged36px row. Actual privatefont16 and exactone-line
patch difference checked; git apply --check PASS. Not native/fallback/all-language
fit. Build/Content notified; no product roots changed.
Content `testing/combat-source2-redraw1/RESULT.md` actually read: exact4file
reconstruction/source2+overrides and12context/reentry models PASS, no concrete
new defect. User also reports row32-readback PASS with conditional16px font scope.
Preferred final text-fit patch now `research/combat-source2-on-50f07708-textfit.patch`:
ONLY additional footer height42->48 against row32. Three explicit Small16 lines
measure272/378/463px within516width; need48height, old42clips6. Ends486<500,
right532<cancel548. Application/exactone-delta checks PASS. Content asked to review
ONLY this footer delta; no repeated12model audit. All older patches preserved.
Content footer-readback.json now actually read: single42->48 delta PASS,
3x16 lines fit, bottom486, cancel gap16, text/reentry unchanged. Widths remain
explicitly Frontend measurements, not independently reproduced by that review.
No native/all-font acceptance or root application.

Content50f package gate actual summary read:
`testing/windows-50f077-audit/final-summary.json` PASS static package/source/CRT/
privacy, releaseHELD. ZIP ee2589865c6dc64cf9ed196e1b5d7dc8e11b6da43687e2c01bf5002e9ae92015;
85CIpackage regressions/0fail/0skip. Native B/C/context/fullredraw/save remain unrun.
No duplicate whole-package audit performed by Frontend.

NEW MATERIAL CLIENT FIX: owned ROOT `client/battle/BattleHeroActionWindow.cpp/h`
now adds showAll override calling refresh() before CWindowObject::showAll. Actual
WindowHandler full-redraw paths invoke showAll, which formerly bypassed show-only
availability/effect refresh. Activation guards unchanged; existing9spell mutants
PASS and both redraw entry bodies checked refresh-before-base. SOURCE ONLY, not
compiled/native/reentrancy acceptance. Content review requested. Build notified:
these2root bodies changed, so immutable source1/source2 ROOT-BASE checks must be
explicitly rebased/merged with this additive fix; never bypass pins or mutate offers.
No art/rules/CMake/profile changes or GUI execution.
Build now holds all six source1 client paths for explicit routing+showAll merge,
keyboardB/English pairing and existing Windows FULL route. Frontend does not edit
those paths during integration. Persistent test update outside hold:
`client/tests/check-hero-action-spell-routing.py` PASS9activation+4missing/late-refresh
mutants. Content notified that GUI-thread CIntObject::redraw synchronously invokes
showAll; cache-before-redraw setters inspected, recursive rendering/native follow-up
not claimed proven by source checks. Content actual
`testing/orders-full-redraw-current1/RESULT.md` read: exact additive override and
four synchronous-reentry models PASS, no concrete defect. Qualified base has no
show/showAll cycle; text/cache/state updates precede nested redraw and converge.
Not native lifetime/thread proof. Build's immediate route remains source1 split;
future source2/Focus rebase requires its own effects/context gate. Required native
checks include full/pending redraw, uncover/resize, changed budget/turn/tactics/
autofight and expired context, without stale enabled actions or unwanted requests.
Content integrated source-pairing PASS now read at
`testing/combat-routing-integration1/RESULT.md`: exact10-file candidate, six client
bodies source1+ONLY additive showAll; B/English-only config changes, C Spellbook and
controller mappings unchanged;9+4source mutants and3binding tests PASS. Source1
null-spell guards/reentry qualification retained. Explicitly NOT source2/Focus.
No concrete pairing defect; eligible for Build compile, not native execution or
visual approval. Held six paths remain untouched by Frontend pending Build release.
ACTUAL Build handoff now read: scoped commit50f07708caf87ac7d2c7ce1a6088a59d11d61bac
pushed by Build; Windows FULL34721537809 now TERMINAL SUCCESS through unchanged
workflow. Actual `build/combat-routing-integration1/terminal-query.json` parsed:
completed/success, exact50f07708caf87ac7d2c7ce1a6088a59d11d61bac,
updated2026-09-12T22:47:24Z. Changed artifact/package gate and native gameplay
remain pending; this is not publication or final UI approval.
Finalized download summary read:143.43s/raw API digests+CRC PASS, no retries.
Frontend then read ACTUAL finalized source tar and player ZIP under
`build/combat-routing-windows-download1/10306544640/`: six changed client bodies
plus archived regression checker match committed50f07708 after CRLF normalization;
archived chooser activation/redraw assertions PASS. Both shipped changed resources
(keyBindingsConfig and English binding translation) also match that commit after
CRLF normalization. This is explicit normalized text agreement, NOT byte identity.
No duplicate download/extraction tree or native launch; complete package gate stays
Content-owned and release-held.
`https://github.com/thegandalf196/vcmi/actions/runs/34721537809`
Existing195-minute watcher in `build/combat-routing-integration1/` wakes named
HoMM3 workers on terminal result/monitor failure; terminal wake received.
No local compiler/GUI launched. Do not duplicate dispatch or cancel. Next: inspect concrete
failure or independently gate changed artifacts, then required native acceptance.

INDEPENDENT WORK RESUMED by user: Hero art/ability uncertainty does NOT hold
QS/QL/Charge or combat routing. Actual QS merged-source1 and Charge mapping-source1
already delivered; Build `convenience-six-school-delivery-audit1.json` reports both
six-school2 stages still lack this repair. No matchedCharge50 found in external
outputs. Combined plan remains; no B64 substitute, no QS-only permission inferred.
Concrete next combat integration route sent HoMM3:Build: immutable
`research/combat-entry-split-source1` identity27d566bad60c0d8c5b14e3061ae523b79c0b412fecefda1462483bff79a276dd,
6 existing client bodies, no newCPP/CMake/Runtime4 dependency. Pair Build-owned
keyboard.battleOpenOrders=B and binding localization (never controllerB). Use only
an actually admitted clean compile route; no blocked Linux restart or GUI launch.
This canonical single-dispatch/native Spellbook/bookless Orders slice uses existing
legacy520 placeholder art, NOT rejected B. Source2/Focus/full Hero are retained
future scope, not cancelled. No duplicate source slice/guard framework created.

GREY INTEGRATED / FRESH QS VERIFIED: all3 actual1381e30c2 Gitblobs match9cafoffer.
FreshBuild `build/qs-adaptive-current-source1/identity.json` 38members personally
read/hashchecked: two configs exactreviewedmergedsource1;36art bodies exactsealed
responsive-source3/button-art1. Initialcomparisonwrongextra/files path corrected;
no candidate writes. Existingrecipe5/art2 testsPASS. Contentcurrentrebind/own-art
provenance gate remainsseparate; no nativeplacement/input/rendering acceptance.

USER GREY/QS SCREENSHOTS INSPECTED: personally viewedprivate spellbook-grey-panel.png
andquick-save-load-position.png. Grey is actualopaque schoolTabPanel code, not an
assetoverlay omission. Fixedin exact `research/native-spellbook-edge-source1/identity.json`
SHA9caf07d0c0957fcde002f011e6de085ff185471266a524a4d68f0fd176e85456:
CPicture crop ofalreadyplayercoloredactualbackground, same83x294 source/target;
decorativeinputremoved. InstalledSpelBack viewed: no school emblems; largegenerator
also usesSpelBack, legacySpelTab is separate/legacybranchonly. All/6tabs unchanged.
EightfocusednegativecontrolsPASS; Build/Content receivedoffer, notnativeapproval.
QS trace: canonicalstage containsonebaseadventureMap.json plusoldnhConvenience
addon(top171,right69,24pxframes); noadaptiveadventureMap override. CurrentCpp
buildswinningbase thenaddonitems. buildMapContainer supportsactualpos.h conditions
(strictheightMin, inclusiveheightMax); adaptiveexistingrecipe uses thisconsumer,
not image-only replacement. Re-ran sealedrecipe5tests/art2testsPASS. Build askedto
freshlyapplyreviewed `build/convenience-merged-source1` two-config output plusfitted
art; emptynhConvenience.items preventsduplicates. No viewportinferredfromcrop,
noF8/F9change or GUIlaunch. UserexplicitQSrepair supersedespreviouscombinedCharge
artdependency for thisboundedfix; unapprovedOrders/Chargeart stillnotinvented.

USER LINUX770377 RENDER FEEDBACK + ART CARRY-FORWARD REPAIR: user seesnativeyellow
All andnewHero, but commissionedindividualschoolbookmarks reverted. Rendering-only
feedback, notfullMANUALPASS. Frontend independentlyread all162 approvedpreview
members andmatched mapping144 SHA pins; comparedcurrentstage:144PNG+6spellBorders
JSON DIFFER,12bookmark/buttonJSON SAME. Exactread-onlyreport
`research/frontend-school-carry-forward-check1.json`. Missingprivatepayload is
confirmed, not a runtime cause diagnosis. Build preparingNEW privateLinux770377
successor withall162+onlysixborderpointeredits; binary/yellowAll/Hero unchanged.
Neverhotpatchcurrentstage/profile; no needlesscompile. Contentchangedassetcheck
requested. Ordersgauntlet remainsunapprovedart, notregression; no guessedgeneration.
Readactualsuccessor `build/linux-770377-school-overlay1/result.json`: archive
`build/linux-770377-school-overlay1/New-Horizons-Linux-770377-Six-Schools.tar.gz`,
18991114bytes, SHA821c5f85ee093db5c75ec41e92f13180673564087f150cc91b1446745556a69b.
Source770377; result sayssamebinaries/privateonly, independentaudit pending.
Readnew `New-Horizons-Linux-Six-Schools/Play-Six-Schools.sh`: delegatesnormalwrapper
withfreshprofile `$HOME/.local/share/new-horizons-770377-six-schools1`. NoGUI launched.
Contentaudit nowread directly at `testing/linux-770377-art-carryforward1/successor-summary.json`:
PRIVATE_CANONICAL_PACKAGE_STATIC_PASS_NOT_RENDERED, all162exactassets andonlysix
semanticborderpointeredits, sameclient/lib hashes. Archive821c5f85 confirmed.
Readyforprivateuserdelivery withfreshwrapper; notrendered/input/save/publicrights
acceptance. Originalstage checksums/identity/binaries preserved.

LINUX770377 DELIVERED: read actualtesting/linux-770377-audit/summary.json status
PRIVATE_THIN_STAGE_STATIC_PASS_NOT_RUNTIME_OR_PUBLIC_RELEASE, exact77037728fcd23689e0d1642b0780e9453e637bec.
Build handoff records702/702 initial and4/4 finalincrement EXIT0; delivered
`build/linux-current-client1/New-Horizons-Linux-x64-77037728fcd2.tar.gz`, SHA
7305f99d259d54de3ac334df345b8247adc10f71887faaf8b8d710ad40864f93.
Ubuntu26.04-dependent thin stage, not portable/public/native/input/save acceptance.
Windowsparity34797565513 nowregistered atsame770377 perBuild, independentofLinux
delivery; boundedBuildwatch owns terminal/defect wake. Earlierpackages untouched.

ALL BOOKMARK SOURCE2 INTEGRATED: Build reports77037728f committed/pushed,
superseding8359; actualthreeGitblobs verifiedagainstc863source2, allmatch.
Linuxcompile ongoing; mandatoryfinalincrement mustpin770377, no dirtysuccessor
stamping. Compile/result and native input/rendering acceptance remain pending.

ALL BOOKMARK SOURCE2 supersedes1: actual CPicture cropconstructor Images.cpp96
registersLCLICK|SHOW_POPUP evenwithoutcallbacks. Bothdecorativeimages nowexplicitly
remove thoseevents, preservingsoleexisting64x64InteractiveArea input/help.
Exact `research/native-all-bookmark-source2/identity.json` SHA
c863b7ebb2de4b8ef3df8e2babae6123c01762619ff114d963286c84b7de7901 delivered
Build/Content immediately;6negativecontrolsPASS. Source1preserved, notcurrentoffer.
No changes to crop/frame/layout/resources/art. Nativeinput stillunverified.

USER LINUX ALL BOOKMARK FIX READY: replacedcustom-All placeholder consumer with
runtime purchaser SPELTAB crop(0,236,83,57), frame0inactive/frame4selected, at
(524+offR,324). Personallyviewed both; installedH3sprite archive/resource identity
matchesprivate priorinventory. Sixcustomschooltabs/art/layout unchanged; retained
existingAll64x64hit area(534+offR,318) andhelp458, canonicalselectSchool(ANY).
OnlyCSpellWindow.cpp/.h + focusedsourcechecker; 4negativecontrols PASS, not compiled/
native rendering/input evidence. Exploratoryassert all0..3inactivecropsidentical
FAILED(frame2differs); not a relied-upon premise; preserved qualification.
Exact `research/native-all-bookmark-source1/identity.json` SHA
321d1b19afe7d8a3ff491fad28110290e4880bfd709497bfc3ae7ea3bb1ac35d delivered
Build/Content forpromptfocusedreview/Linux integration. No proprietarypixelcommit,
newAllart, toolchain/guard work orGUIlaunch. UserexplicitlyauthorizesnormalLinux
configure/compile/package; Build owns it andmuststatecoherentcandidateidentity.

POLISH DOWNLOAD: actual `build/hero-polish-windows-download1/summary.json` read:
141.7313s/no retry,3artifactdigests/CRCs PASS, explicitly NOT_PACKAGE_AUDIT.
Build suppliesplayerpath
`build/hero-polish-windows-download1/10326954262/New-Horizons-Windows-x64-48e45a45d4c4.zip`,
25283935bytes, SHA f97bc9228653abe8e62e54af1007c9139c493405d7cc72d6f0006c504b417e4b.
Content audit pending; no duplicate download or native/input/save approval.

POLISH BUILD TERMINAL SUCCESS: actual `build/hero-polish-build1/terminal-query.json`
verified34785626669 completed/success at48e45a45d4c456098d5e9753cafbf09cabdebf76.
Boundarypolish compiles; native rendering/seams/obscuration, input/save, packageaudit
and finalart/publication acceptance remain separate and unproved.

POLISH BUILD ACTIVE: actual `build/hero-polish-build1/current-query.json` verified
FULL34785626669 in_progress at48e45a45d4c456098d5e9753cafbf09cabdebf76.
Actual4b07..48e45 changed-path list: ONLY client/render/AssetGenerator.cpp.
Existingroute/TestsOFF; boundedBuildwatch owns failure/terminalwake. Priorpackages
untouched; no rendered/native/save/artacceptance inferred.

APPROVED AFTER BOUNDARY POLISH IMPLEMENTED: personally viewed exactprivate
hero-polish-approved-direction-FjXIS4u.png AFTER panel; scaledboard is direction,
not pixelgeometry or productpixels. OneAssetGenerator.cpp change: native recessed
cellbevels plus stronger equipmentwrapper/tray/skills/army/rail boundaries. Same
800x624/resources/palette, no control/value/font/hitbox/emptyrow changes, no added
presentationtitle/outerdecor or artgeneration. Exactoffer
`research/hero-boundary-polish-source1/identity.json` SHA256
f9f5437d62a8c1a945c739615fe874a4c2c1aabb86598c99de8467605b145531 sent
Content/Build forchangedscopereview. Hero8/11source controls and5section boundsPASS;
Build integrated/pushed48e45a45d; actualcommittedbody verifiedagainstf9f543offer,
match. Sourceholdreleased. Not compiled/nativefit/artfinal acceptance; rendering,
seam/obscuration andsave gates remainunrun. Existing4b07build staysunchanged and
excludespolish; latercompile needs ownidentity.

EMPTY-ROW BUILD TERMINAL SUCCESS: actual `build/hero-empty-row-build1/terminal-query.json`
read:34782388008 completed/success at4b07b0de8469f41d6ef17554bbf45fe7cf1b860f.
Empty-row cleanup compiled; excludes48e45 boundarypolish. Not native/UI/save/art,
packageaudit/publication or V2activation acceptance.

EMPTY-ROW BUILD ACTIVE: actual `build/hero-empty-row-build1/current-query.json`
verified FULL34782388008 in_progress, exact4b07b0de8469f41d6ef17554bbf45fe7cf1b860f.
Actual9ccd..4b07 changed-path list is ONLY CHeroWindow.cpp/.h. Existingserialized
route/TestsOFF; boundedBuildwatch owns failure/terminal/download wake. Audited9ccd
unchanged; no native/UI/save/art acceptance or V2activation inferred.

ACTUAL USER HERO RENDER: personally viewed private
`HoMM3-art/references/user-ingame/hero-9ccd-user-IGwcuNL.png`, SHA256
07dcdf8d28fc0324e031a758330995cff2d33a2e00b4e6fdc3b63eabce7041ba (1242x976).
User reports9ccd and noadditionaloption: KorbacL1 Beastmaster, live15/20/5/10,
23/750leadership,1339/1560movement,8rows,Backpack/noCommander visiblyrendered.
This is real user-rendering evidence, not independentexeidentity,input/save or
fullMANUALPASS, and grants no workerGUIpermission. No optiontoggle requested.
Bounded2file cleanup nowimplemented: onlyplaceholderlabels/questions hide on
unlearnedrows, 24celloutlines/help and8rows retained; freshskillcount onrefresh,
legacyfallback unaffected. ExistingHero8/11+inactive3sourcechecks and0/2/8 visibility
models PASS; exact2file frozenoffer `research/hero-empty-rows-source1/identity.json`
SHA484d5616752bd55a04a73b590d2c437c4557568598d8d2bf07fc8f0530ba298a supplied
forContentbinding. Build integrated/pushed4b07b0de8; actualtwoGitblobs verified
against484didentity, bothmatch. Sourcehold released; source-only cleanup, not compiled/
native acceptance. Frozen9ccd package and userimage unchanged; any successor build
needs its own explicitidentity. SiegeA0B0F0
andTBD remainreviewitems. Fixedblueinner comes fromexplicitblue texture/equipment
color1 whileBORDERED frame usesplayercolor; no blanketcolorbug or policychange.

NEW USER-REQUESTED ORDERS VISUAL DELIVERED (independent ofpackage/native waits):
`research/orders-native-material-preview-private.png`, ONE668x640 review sheet:
640x500 actualconditionalV2 panel +nativeDIALGBOX exterior, separate unscaledtoolbar
excerpt. Personally viewed finalimage. Nativebrown/256blue sharedplanes/subtlewells;
actualICM005Spellbook/ICM006Wait/ICM007Defend andbutton80Targets. Explicit? placeholders
forunapprovedgauntlet/Orderart; labeledCancel placeholder. No rejectedA/B authoredart,
newicon generation, gameGUI/import/build. V2illustrative only,currentconfigstillV1;
realaction roster/sharedbudget/booklessOrders preserved. Conciseactions/art/fit
manifest `research/orders-native-material-preview.md`; allshown nativefont widths
fit, realnumeric/localized/nativefit stillunproved. This is MOCKUP, not finalart.

9CCD INDEPENDENT AUDIT NOW READ: actual `testing/windows-9ccd51-audit/final-summary.json`
PASS package/source/CRT/privacy, RELEASE_HELD. PlayerSHA
11984c4ade6ea0ce1469794d5867e054662b5d8b962445fda9c91b5d8739b8c2;
1213files/1212sums/26PE/6172imports/4738sourceblobs;87packagechecks0fail0skip,
CRLF/120source-mode differences qualified. No further unchanged-byteaudit needed.
Build's current explicit route state: no admitted test-enabled/native64 or compatible
Linux runner. Actual in-game validation needs a newly authorized Content Windows
runner with pinned licensed corpus/staging, OR a new compatible Linux build/profile/
session admission. Oldguards do not apply. Compile-onlyPRE_TEST remains proposal,
not native proof. No route or permission inferred from offlineOrders preview.

9CCD DOWNLOAD READBACK: actual `build/focus-hero-windows-download1/summary.json`
read: sole download133.7895s, no retry, three artifact digests/CRCs PASS. Mainartifact
10322768601 rawSHA0100973785c16c82c2296749c38493e81407578d7979cda22e31e026cb135825.
Status explicitly NOT_PACKAGE_AUDIT; independent Content audit pending. No duplicate
download/helper execution or native/publication claim.

CORRECTED BUILD TERMINAL SUCCESS: actual `build/focus-hero-link-repair1/terminal-query.json`
read:34771438399 completed/success, exact9ccd513dcfc7677fa51066d20f0bcb4cfd99a898.
Combined Focus+Hero compilation/link milestone reached after preservedC2039 and
missing-registration failures. TestsOFF: not the64nativecase gate, nativeGUI,
V2activation, package audit/publication, save integrity or finalart acceptance.

CORRECTED BUILD RUN: actual9ccd513dc commit inspected, only2client/CMakeLists
registrations forFocusFireTargetWindow.cpp/.h. Actualcurrent-query for
`build/focus-hero-link-repair1` shows FULL34771438399 in_progress at
9ccd513dcfc7677fa51066d20f0bcb4cfd99a898. TestsOFF; boundedBuildwatch owns
follow-through. Newselectorobject stillrequiresactualcompile/link result. Not
unchangedretry/isolated5c/native/package acceptance; failedattempts preserved.

COMBINED BUILD LINK RED: actual34769181914 terminalfailure atde1bb7cd0;
`build/focus-hero-successor-integration1/failed.log`771/773: unresolved
FocusFireTargetWindow(shared_ptr<BattleInterface> const&) /LNK1120. Actualheader
anddefinition match; explicitclient/CMakeLists hasBattleHeroActionWindow but lacks
FocusFireTargetWindow.cpp/.h, andlog hasno selectorobject. Build checking owned
registration repair; no Frontend CMake/signature edits or unchangedretry. Thisrun
does not compile-test the omittedselector. PriorC2039 notreported; no nativeclaim.

EXPLICIT COMBINED SUCCESSOR: actual current-query verified Windows FULL34769181914
in_progress atde1bb7cd0a965a03a051e9171a9ab34d006d412b, under
`build/focus-hero-successor-integration1`. Build identifies CURRENT-SOURCE Focus+Hero
including reviewedC2039repair/inactivefix/AIchanges, TestsOFF. NOT isolated5c repair
or unchanged retry. Failed5c and isolatedrepair preserved; boundedwatch willwake
failure/terminal. No native/V2activation/publication/64nativecase acceptance.

HERO COMPILE RED / BOUNDED FIX: actual34766507725 terminalfailure at5c169;
`build/hero-preview-integration1/failed.log` line706 reports MSVCC2039:
CToggleBase has no moveTo. CurrentrestoreLegacyLayout's two formation entries are
constructor-created CToggleButton instances stored through state-onlyCToggleBase.
Fixed ONLY CHeroWindow.cpp: static_pointer_cast<CToggleButton> forboth entries before
move; nonvirtual inheritance and concrete construction inspected. Two casts+comment,
allother source unchanged. Hero8/11 +inactive3 source controls PASS; diffcheckclean.
Content boundedreview requested; Build owns correctedcommit/FULL and must explicitly
choose sourceisolation (currentHEADincludesFocus), not silentlyretargetfailedHero.
Failure/snapshots preserved. Content independentlyconfirmed mismatch and recorded
its earlierAPIreviewmiss. Exactonefile `research/hero-toggle-cast-source1/identity.json`
SHA64ade310400866f17aaa7c17d920c477d19fe1131c3c45446cedefb3d9af5b7e supplied
forboundreview; includes already integrated inactivefix, onlynewdelta2casts/comment.
Repair not compiled/native accepted yet.

HERO INACTIVE-RESIZE SUCCESSOR (2dirtyfiles, not frozen5c): actual inheritance
trace found CWindowWithArtifacts::updateArtifacts writes global dragcursor and
calls artifact hover(true); CHoverableArea writes current ENGINE statusbar without
activeguard. Active-only replacement registration did not prevent these subsequent
writes during inactiveHero resize. CHeroWindow.cpp/.h now separate refreshHero(bool):
ordinary updateArtifacts passestrue, resize passesisActive(); localvalues always
refresh while inheritedglobalinteraction work is skipped forinactive resize.
`research/check-hero-inactive-resize.py`3mutants PASS; previousHero8mutants/11models
PASS. Content review requested, Build notified; frozen5c offer and runningisolated
Hero34766507725 unchanged (actualcurrent-query verifiedin_progress atfull5c hash).
Content confirmed the source trace and requested frozenbinding. Exact2file offer
`research/hero-inactive-resize-source1/identity.json` SHA256
f8759d413aa6d942fb69df13cec049f210fa9e17dfcc6fcd26fc9dc05addc91b now supplied;
actual3mutants PASS fromsnapshot files. Build reports independent3controls accepted,
committed/pushed7569185a1; actualtwoGitblobs verified againstf875identity, bothmatch.
Sourceholds released. RunningHero34766507725 remains5c169 andEXCLUDESthisfollowup;
no retarget/cancel or nativeacceptance. Await actualcompile result separately. No compiled/native/modal/
cursor proof. This is a new successor, not retroactive5cPASS.

MODEL-STATE WINDOWS RESULT: actual `build/model-state-integration1/terminal-query.json`
read:34763490175 completed/success at6fc2e9829b2e8720c3f2d51fd2521991a8011953.
This predates Hero5c169 and excludes the unmerged Focus successor. No Hero compile,
gameplay, native fit or publication acceptance inferred.

HERO INTEGRATED: Build committed/pushed5c169e08a; actual six Git blobs verified
against573afb frozenidentity, allmatch. Source holds released. Existing6fcCI
unchanged; Build willpin separateHero source-preview identity under authorizedroute.
Not compiled/native/final ability/art acceptance; existing acceptancegates remain.

FROZEN HERO SOURCE REVIEW: `research/hero-consumer-source1/identity.json` SHA256
573afbb45c33f81aac47948b0d5c39ccf8a253dced97f9951c010007d96cbcc0 binds6client
bodies pluschecker. Ranchecker FROMsnapshot files: PASS8mutants/11creation models
and retention/order/registration assertions. Old4file Content checkpoint actually
read but NOT promoted to cover new6file resize/statusbar implementation. Exact6file
review completed: actual `testing/spell-target-control-current1/HERO-SIX-FROZEN-REVIEW.md`
read, bounded SOURCE PASS matchingidentity/all6hashes. No additional source defect;
active-onlybar registration, backgroundorder, retainedholders/slider/label/API paths
reviewed. Sent Build source readiness for scoped integration/isolated Windows preview
decision under existing route; review itself grants no compile/GUI permission.
Roots remain held pending integrationfeedback. Native picked-artifactresize, modal
bar ownership, fit/transitions/localization/save and in-gamecohesion remain gates. Existing
Focus patch, current6fcCI and prior packages unchanged. Preserve this offer.

FOCUS INTEGRATED4596dfe1f: actual commit shows46paths total and exactly4client
paths (chooser.cpp/.h, FocusFireTargetWindow.cpp/.h). Acceptedtarget-help patch
passes reverse-apply check againstcurrentroots. No otherclient paths changed in
this commit; Hero/inactivefix/Ordershelp/quickslots preserved. Actualpost-merge
Orders9+4+3 and caster5+quickslot8 source controls PASS onintegratedroots. Requested
Build's concrete next test-enabled lane decision for amended64 Focus cases using
`*FocusFire*:LegacyCommandAllocationTest.*`, with otherregressions kept separate;
no duplicate/automaticdispatch or nativeclaim. Build reports46blob
assembly match; Frontend verification here is scoped toclient paths/patch, not all
Runtime bodies. ActiveHero34766507725 remains5c169. No newGUI/native acceptance.

FOCUS WORK5 PAIRING: current declaration-compatible client remains
`research/combat-source2-on-50f07708-target-help.patch`, SHA256
`a4915f9ea56f9a8c38774386ef12b92a68caed30acfc37738c08c897c0945199`.
Actual Runtimework5 six declarations match and FocusFireState unchanged from4;
git apply --check PASS. NOT old work5/client2 wholesale copy. Four chooser/selector
paths only, preserving658/706 BattleWindow and six-file HeroWIP. Runtime/Build
notified. Actual sealed Runtime5 nowread/verified: identity
f31a31e4677cacb8e1ddef1d4d9a3195ce65b89865142e140bd0fb494c908bf4;
all45members match; three interfaceheaders byte-match inspectedwork5. Build notified
of sealed pairing, not automatic root apply or compile/native GO.

REAL HERO IMPLEMENTATION IN PROGRESS (not source-ready): Build cleared exact
CHeroWindow.cpp/.h and optional existing AssetGenerator.cpp/.h ownership. Runtime
confirmed existing read-only hero getters/callbacks, no schema/save migration;
Siege must say existing/legacy capability, NOT spendable balance. Retain legacy
Mastery/development access, >8skills/small-viewport/optional-mechanic fallback.
Started resource compositor in AssetGenerator.cpp/.h:800x624 brown native texture,
actual engine-filtered blue resource with shared origin and translucent wells.
No flattened/private image import. Consumer now wired: creation-time844x668 logical
viewport includingframe/shadow margins, savedgrowth/<=8skills/noCommander/nonRoE and
UI-enhancements-enabled gates; legacy fallback otherwise. Content caught actual
nullBackpack with enhancementsoff; fixed predicate to match control creation.
Eight skill widgets/24 unbound cells with help (not ability mechanics), actual
Backpack and existingdevelopment access; livegrowth/capacity/movement/mana and
explicitlegacySiege A/B/F ranks. Garrison refresh updates capacity, onearts holder
retained under existing !arts guard. Native equipment crop by resource, no scaling.
`research/check-hero-consumer-source.py`:8fallback mutants/11creation models PASS;
existing mastery routing2controls PASS; diff whitespacecheck clean. Initialchecker
mistook slider callback for final initialization; corrected checker, not product.
Content four-file source review requested; NOT source-ready for integration yet.
Found actual resize gap: inherited onScreenResize only recenters, so creationgate
alone could clip an open new window. Build ACKed6file expansion CWindowObject.cpp/.h.
Implemented protected setBackgroundPresentation with presentation-only mask; existing
callers unchanged and popup/input flags retained. IN-PLACE restoreLegacyLayout keeps
samearts/artSets+garr, restoresnative controls/background and >8skill slider; no
window pop/recreate or resolution mutation. onScreenResize falls back beforecentering;
refresh detects eligibility change too. Legacy initialresize remainscenter-only.
Localizedstaticlabels now retrim aftersetMaxWidth; originals restored onfallback.
Six-file Content review requested. Further concrete source issue fixed: createBg
appends replacement background, while showAll draws children in order. Presentation
setter now rotates only the new background to the first child, preserving retained
control order/shadow tail; generic setBackground callers unchanged. Content found
live statusbar registration gap; fixed by statusbar->activate() AFTER replacement
only if Hero isActive(). Actual CGStatusBar activation registers shared ownership;
base activation is idempotent. Inactive underlying windows do not steal modal bars.
Source/order/registration assertions PASS. Source fallback/retention assertions PASS, not
nativefit/hitarea/resize/transition proof. Still NOT integration-ready pending review.
Actual fb829 Windows terminal34760509964 success read separately; excludes HeroWIP.
Native Content execution still needs a separately valid route; no blanket GUI grant.

WINDOWS BUILD UPDATE: actual `build/spell-ai-integration1/terminal-query.json`
read: FULL34757691605 completed/success, exactedc975615de368b1f3d1542b7b56656d30aa92ee.
Not evidence for later658f Orders help,706quick-slot guards or unmerged Focus/Hero
preview. No gameplay/publication acceptance inferred.

LATEST HERO PREVIEW — USER800x624 GEOMETRY APPROVED, superseding viewport/semantic
hold below: one composed `research/hero-800x624-composed-private.png` delivered;
editable recipe `hero-800x624-preview.py`; readable `hero-800x624-text-overflow.md`
and JSON metrics. Personally viewed final800x624 image. Eight44px skill rows,
24ability placeholders, nativefonts/footprints; no final displayed truncations.
Actual52x36heroBackpack configuration and45x33native overlay reused, no Pack text;
Commander omitted, NOT replaced with castellan. Shared256brown/filteredblue planes,
subtle empty-well shading; existing native equipment region retained. Leadership,
Movement, Siege explicitTBD icon boxes. No invented ability roster/eligibility or
Siege economy. Correct native morale+1/luck0 frames4/3. No previous previews changed,
new art family, product imports or GUI launches. Geometry approval is not this
composition's finished-art/rules/runtime/public-rights/small-display acceptance.

QUICK-SLOT INTEGRATION UPDATE: Build reports scoped commit/push706d26bdc of
exactly2reviewedfiles;5+8controls rerun PASS. Actual git commit inspected; latest
`combat-source2-on-50f07708-target-help.patch` still passes git apply --check on
current roots. Its4paths unchanged50f..706; it does NOT touch BattleWindow or caster
checker, so patch-only application retains658f/706. Do not recopy the other4 old
source2 bodies. Build notified; no new offer copy/root apply. Source hold released; no separate
FULL/GUI and activeedc CI unchanged. Future Runtime4/source2 merge must retain
currentHero/bounds/retarget guards AND658f read-only Orders help. Frozen packages
unchanged. This is integration evidence, not new compiled/native acceptance.

NEW INDEPENDENT COMBAT CODING (Hero composition hold does not apply):
Current roots inspected; disabled Orders help already committed by Build658f9991e.
Implemented fresh quick-spell slot activation guards in BattleWindow.cpp: reject
replaced battle/null interface/autofight/tactics/foreign turn/missing panel before
reading roster; snapshot and bounds-check index; currentHero feeds unchanged
canBeCast and owner.castThisSpell path. No spell-targeting-mode ban added, preserving
valid quick-slot retargeting. No direct budget/game-state mutation. Extended
`client/tests/check-spell-caster-routing.py`:5existing caster+8quick-slot guard
mutants PASS; existing16Orders checks also PASS. Build/Content received explicit
2file root delta. Content actual `testing/quick-slot-activation1/RESULT.md` read:
SOURCE/checker PASS5+8; context/bounds precede access, positive caster route and
retargeting preserved, no new defect. SpellID validity remains the roster producer's
existing invariant, not arbitrary-ID validation. Native valid-slot/retarget/cancel/
stale context and duplicate-dispatch checks remain unrun. Not compiled/native
accepted; no Hero/rules/art/GUI changes.

LATEST USER SEMANTIC HOLD: stop next full Hero/art composition until icon/control
inventory is settled; independent combat/backend coding is NOT held. Pack is
createBackpackWindow/heroBackpack: use Backpack or its genuine icon, not obscure
Pack. Commander is conditional hero->getCommander(), an optional commander CREATURE
opening CStackWindow; NOT Orders, castellan or governor. No new1.0Commander inclusion
is authorized. Persistent placeholder in mockups is misleading; recommend omit
from default NH mockup unless that supported mechanic is enabled; disposition pending.
New distinct art needed for Movement, Leadership, Siege; ability art waits for actual
roster; Orders/Doctrines and separate gauntlet remain distinct. Reuse unchanged
native XP/mana/morale/luck/primary resources. Existing Siege image is only a candidate.
New blue direction accepted, not full composition. No artwork generation batch.

LATEST BLUE STUDY delivered STRIP ONLY, not another fullUI:
`research/blue-strip-material-study-private.png` plus720x64 standalone
`blue-strip-filtered256-private.png`, editable `blue-strip-filter-study.py` and
method JSON. Read actual AssetGenerator getColorFilters/createPlayerColoredBackground,
ColorFilter.cpp and SDL2 ScalableImage palette rules. Blue parameters
[0,0,0,0.45,1.20,4.50] produce diagonal float32 RGB multipliers, truncate to int,
clamp0..255; OPAQUE alpha and skipmask0. Eight special palette entries are skipped
on abs-channel-diff<8; NONE are used by this DiBoxBck source. Raw indexedPCX decode
matches existing privatePNG. Actual native53x56 rail interior also shown unscaled,
NOT expanded/repeated; initial taller sample exposed a lower rule and was trimmed
before final delivery. No clean720x64 contiguous source identified in boundedstudy.
Filtered256x256 tile is displayed with its actual256px repeat, origin12,520, not32
repeat/stretch. Personally viewed actual strip/sample; this does NOT prove visual
cohesion or native renderer parity. Prior previews/approvedbrown/layout unchanged;
no generation/import/GUI. User review of strip remains required before fullUI.

NEW INDEPENDENT ROOT INPUT/DISPLAY PATH IMPLEMENTED after user continuation:
`client/battle/BattleWindow.cpp` gives the disabled Orders toolbar entry read-only
right-click help with freshly evaluated battle/phase reason. blockUI restores ONLY
SHOW_POPUP after blocking; mouse issuance and B remain blocked as before. Popup
checks current battle/interface/controller before phase reads, issues no request,
and generic help is empty to prevent duplicate popup. No new art/rules required.
Existing `client/tests/check-hero-action-spell-routing.py` extended: actual
9activation+4redraw+3click/key/dispatch mutant checks PASS. Build/Content notified
of explicit2file live delta.50fcompiled commit/artifacts and frozen Focus patches
untouched. Content actual `testing/orders-windows-regression1/DISABLED-ORDERS-HELP.md`
read: SOURCE PASS, no new defect. addUsedEvents respects active/inputEnabled;
SHOW_POPUP alone restored, no click/B; empty generic help avoids second popup.
Tactics-disabled widget stays disabled, so its reason is not necessarily reachable.
Native popup/dismissal/context/blocked click+B/unblock/lifetime remain unrun.
Separate from test-only commit and frozen50f package acceptance.
Coherent-blue material task already delivered below; no duplicate batch or viewport
approval inferred while implementing this independent path.

LATEST BLUE CORRECTION — previous blue-only result rejected as block collage.
Completed ONE successor at OLD800x600 geometry:
`research/hero-blue-coherent-private.png` and
`research/hero-blue-coherent-before-after-private.png`; editable
`research/hero-blue-coherent-repair.py`. All army-strip blue now comes from one
native32x32 2D plane/common phase, INCLUDING slot interiors; no opaque native-well
copies. Uniform translucent well shading and thin bevels overlay that plane.
Original foreground text/icons/controls/state layers recomposited unchanged.
Actual changed-region assertion confines differences to(12,519)..(732,584);
approved brown, status and all outside pixels identical. Personally inspected
native-size result. Prior previews preserved. User approval of this result remains
pending;800x624 viewport NOT approved, no import/generation/GUI.

Other UI actual status: Spellbook/Orders split+showAll compiled/packaged50f07708,
independent package PASS; native B/C/context/redraw/save unrun, releaseHELD. Shipped
Orders-only chooser still uses legacy520 placeholder layout. Source2/Focus and
textfit patch are source/model reviewed, NOT integrated/compiled/native accepted.
QS/QL adaptive mergedsource andCharge mapping are delivered, not in six-school2
packages; combined route still lacks approvedCharge50, no QS-only permission.
Independent source task IMPLEMENTED as successor patch
`research/combat-source2-on-50f07708-target-help.patch`: retains textfit, changes
only new Focus CPP to add popup-only476x36 text help area,12px clear of Select.
Weak context and exact value ID reacquired at popup time; expired context produces
inactive explanation, not stale pointer access. No CanConfirm gate for reading,
no LCLICK/selection mutation or gameplay request in help callback. Existing states/
row layout/confirmation validation unchanged. git apply --check PASS, compiled
roots untouched. Content actual `testing/combat-source2-redraw1/TARGET-HELP.md`
read: SOURCE PASS, exact FocusCPP-only addition, popup event/weak-context/valueID/
inactive fallback and no selection/dispatch mutation confirmed. No new defect.
Native gesture/dismissal/disabled text/scroll/left-click isolation remain unrun;
no keyboard accessibility claim. No old-model replay. Not compiled/native.
This provides read-only full-target help on Focus rows independent of disabled Select. Current CButton blocking removes popup events;
long clipped target descriptions should remain inspectable even when selection
is unavailable. No new art, ability/castellan/Siege rules are needed for this.

LATEST EIGHT-ROW REQUEST — ONE wireframe delivered:
`research/hero-eight-row-wireframe-private.png` at800x624 logical; editable `.py`
and exact mapping `research/hero-eight-row-wireframe.md`. All8skill rows/24ability
cells simultaneous, NO scrolling/two-column skill layout. First compacted upper
info from2colsx3rows to3colsx2rows44px; all6fields retained, Siege beneath mana.
Kept native44skill/32ability icons (empty wireframe outlines), BIG25/MEDIUM20/
SMALL16 fonts. Removed unused gaps; minimum under these footprints is
88+88+16+352+64+16=624, so800x600 is24px short. Explicit800x624 proposal, not an
assumed approved viewport or global scale. Native equipment/army/Split/other
controls retained; all drawn labels pass native-font width checks. Actual-size
wireframe inspected. No final art, production pixels, gameplay or rules change.
Native brown/blue scopes and previous previews remain untouched.

LATEST USER MATERIAL DECISION + COMPLETED BLUE-ONLY REPAIR:
User approves native brown in the RIGHT `hero-material-comparison-private.png`
image, rejects brushed bottom blue. Repaired THAT approved comparison, not the
unapproved boundary2 experiment. Actual culprit was A's1px column repeated720wide.
`research/hero-blue-only-private.png` and
`research/hero-blue-only-before-after-private.png` now use actual native32x32 blue
rail interior from HEROSCR3(614,8,646,40), inspected: no border/well. One common
origin(0,0), no stretching/generation. All seven complete army frame/well resources
and foreground pixels (icons/text/controls/states) preserved. Pixel checks PASS:
only exposed blue in bounds(71,520)..(732,584) changed; EVERYTHING outside the
repair mask, approved brown, top and status region unchanged. Actual source tile
and corrected preview personally viewed. Editable `research/hero-blue-only-repair.py`;
source sample `research/hero-blue-native32-private.png`. Previous previews intact.
Private offline result, no product import/GUI. Dispatcher notification is this
handoff, not tmux user-chat. The unfinished boundary2 contour experiment is NOT
approved and was not used; equipment transition remains separate pending work.

LATEST MATERIAL DIRECTION: abilities/Siege B rejected; no generated leather or
full redesign. Read actual private `references/interface-native-study/README.md`
and current CFilledTexture::showAll: native tiling begins at each widget pos;
separate fills reset grain phase. Completed ONE private material-only comparison:
`research/hero-material-comparison-private.png` (A/nativeDiBoxBck side by side),
`research/hero-material-native-dibox-private.png` and editable
`research/hero-material-comparison.py`. All A icon/state/text layers reused unchanged;
A reconstruction exactly matches original screenshot bytes. Common256px material
plane at origin0,0 under connected brown region; native frame/rails/thin rules
preserved. Personally viewed result. Equipment's coherent private baked composition
is intentionally retained; its material join is NOT solved or approved by this
comparison. No wholesale extraction/import, font/layout revision, generation or
GUI launch. Future runtime use references installed DiBoxBck through ONE shared
parent plane, not per-cell CFilledTexture fills; extracted pixels remain private.
This is offline material comparison, NOT native game rendering or final art.

VERSION1.0 AUTHORITATIVE SCOPE: read actual `docs/NH_VERSION_1_0_SCOPE.md`.
Track SIX families: primary attributes; secondary skills with3associated abilities
(no wheel, not old masteries); six magic schools; Core/Elite/Champion progression;
Commands; Castellans/governors. Frontend includes corresponding integrated UI, not
rules ownership. Castellan office/mobility/defense/progression contracts are still
unresolved; do not invent controls that imply settled mechanics. No automatic
single-expeditionary-Hero restriction, full Caravan adoption or Siege economy.
Existing code/saves/previews stay intact until deliberate versioned migration.
Labels/family art/source passes are not full feature completion. AI, save integrity,
Linux/Windows, native UI and provenance remain required. No goal reset or new
execution permission; held combat integration paths remain held.

LATEST USER RULE/DESIGN CHANGE — supersedes mastery-cell question below:
Secondary skills now have THREE associated ABILITIES, replacing the intended
mastery design. Heroes V-style rank/ability progression WITHOUT a wheel; exact
prerequisites, offers and versioned save migration remain unspecified. Do not
invent mandatory alternation, activation rules or delete current functional
mastery code/saves before migration. STOP new old-mastery UI/art production.
Siege MAY be spendable; user designs mechanics later. Show an illustrative Siege
panel in the gap under Spell Points, with proposed removal of its top-band repeat;
no invented cost, maximum, refill or duplicate number. Commission reference:
`HoMM3-art/HERO_UI_SKILL_ABILITIES_COMMISSION.md` for faithful Paint main/detail
mockups. User sends prompt to external Codex; no Pi image capability assertion,
Artist ownership transfer, art import or GUI launch. Existing geometry/font work
is historical sizing evidence only, not an ability-rule specification.

LATEST AUTHORITATIVE USER LAYOUT — supersedes our A/B and left-detail-selector
recommendations: personally read `HoMM3-art/HERO_UI_USER_PAINT_DIRECTION.md` and
viewed actual private `references/hero-ui-sketches/user-paint-ivxQY6B.png`1448x1086.
Follow this composition, not another invented direction: continuous full top stat
band with growth markers beside primary icons and morale/luck/siege; compact left
information; SIX visible skill rows, each with skill/rank plus THREE mastery cells;
large equipment at right; player-color hero rail and army/footer. No dashboard tabs
or middle debug column. Whole-image downscaling is not a valid implementation.
Three cells' meaning (all choices versus learned-only) awaits the already-requested
user answer; never infer three active masteries. Six rows are a viewport, not a
skill cap; preserve scrolling/additional skills. Use current saved mastery and
siege/capacity rules, not illustrative names, values, drawn slot count or scalar
Siege. Retain Split and other native controls and one artifact-holder lifetime.
Bounded logical mapping now recorded in `research/hero-user-paint-geometry.md`:
800x600 region allocation preserves full top band, six44px skill rows, native
279x382 equipment union, seven army slots, player-color rail and Split/other
controls. Existing mastery32px assets confirmed (dialog currently uses64px).
Offline current-font follow-up completed: actual private SMALFONT16px metrics
and existing renderer format read. Revised420px row =123px skill +3x93px mastery
+18px scroll; each mastery has32px icon,4px gap,53px text,4px outer padding.
Volley38px/Precision53px fit; Field Repair71px wraps into29px/38px words on two
16px lines within44px height. This is only current ASCII/font measurement, not
native/localized/all-name fit. Full-name help and overflow remain required.
Next dependency is the already-requested user clarification of mastery cells
(all choices versus learned-only), alongside actual supported implementation/
compile admission. No new art batch/import/GUI execution or global scaling. Private mixed pixels remain reference only;
previous batches preserved and B still rejected. Earlier study authorization below
is historical where it conflicts with this user composition.

EARLIER USER AUTHORIZATION — original-led external UI layout STUDY only:
Dispatcher prepares the external Codex prompt against
`HoMM3-art/HERO_UI_LAYOUT_STUDY_BRIEF.md`. Truthful original672x586 baseline;
two800x600 Hero alternatives: conservative integrated character sheet versus
original-language overview plus development page, each with populated main/detail.
User chooses before production. No full asset export, product edits, internal
procedural art proofs, fake GUI/font claims or pretend direct dispatch. Private
original pixels must remain labelled reference. Orders visual pass follows the
chosen language later; separate Spellbook/Orders functionality remains required.
This authorizes the external comparison study, not B adoption or native execution.

USER VISUAL REJECTION — supersedes Revision B readiness recommendation:
B is explicitly rejected, not approved for import or functional-prototype artwork.
Withdraw the proposed B24 command-image overlay; no B art import, visual freeze,
acceptance inference or automatic revision C generation. Preserve A/B and source.
Private rejection record: `HoMM3-art/HERO_UI_REJECTION.md`; original HEROSCR3/4
672x586 backgrounds are privately extracted under `references/hero-ui-original`.
Bounded original-reference comparison now performed: personally viewed private
`references/hero-ui-original/HeroScr4.pcx.png`672x586 and B's actual
`review/hero-overview.png`800x600; read original rejection record and current
CHeroWindow.cpp control placement. This is background versus populated mockup,
NOT a full original GUI comparison. Original keeps left information/right equipment,
a continuous leather field, player-colored right hero strip and bottom army strip.
B hides equipment behind tabs, replaces hero portraits with text navigation,
spreads four primary cards across the width and removes player-color structure.
Recoloring B would not fix these composition differences.

Corrected layout direction for comparison, NOT a new visual freeze: retain the
character-sheet composition and simultaneous equipment/army context; fit growth,
base-versus-effective values and secondary attributes into compact live information
rows, with bounded in-place detail/scrolling for skills/masteries rather than four
large dashboard tabs. Preserve native silhouette/slot relationships and artifact
holder lifetime; do not copy private artwork into original deliverables. Use actual
UI fonts and measured populated content before choosing a larger canvas;800x600
is no longer an assumed approved direction. Actual source additionally exposes
army Split at(539,519), CHeroWindow.cpp current line269; B's drawn footer lacks it.
Include Split alongside formations/tactics/backpack/Commander/journal/dismiss/close
in the next control comparison. No illustrated stat/growth figures are runtime data.
Populated native-layout reference now received and personally viewed:
`testing/linux-413930-readback/01-xp2000-expert.png`; actual `summary.json` read.
It is VCMI413930/packaging83cf with NH ratings and small growth entry, NOT the
unmodified Heroes3.exe.1280x800 capture; no assumed672x586 1:1 scale/font mode.
Visible Orrin L3, eight Expert skill entries in four paired rows, populated
warmachine/equipment region, player-color silhouette/hero strip, army and controls
coexist in one window. Its typography and narrow inset rows preserve information
hierarchy without B's wide card gutters; unlike B Overview, equipment remains
visible while reading all eight skills. Source summary supplies real XP2000,
ratings21/28/7/14 and lastgains3/4/1/2 as reference context ONLY, never constants.

Next composition comparison should keep equipment and army persistent and explore
only a compact LEFT information-region selector for attributes/growth versus
skills/masteries; not a screen-wide dashboard tab system. Preserve native primary
and hero navigation hierarchy, with code-rendered text. Extra base/total/growth
labels must be measured with actual UI fonts rather than assumed to fit old70px
primary columns. Bounded current-source font/density readback: CHeroWindow uses
FONT_BIG for hero name, FONT_MEDIUM for class/level, FONT_SMALL for primary/skill
labels. Native skill region uses four48px rows starting276, two136px columns;
text budgets87px, reduced to71px in the right column when the >8-skill slider is
present at(284,276). Rank and name baselines are20px apart. A selector cannot
simply be added atop this occupied region without explicitly resolving row/icon/
font fit and preserving eight visible skill entries or reviewing the tradeoff.
Do not replace these renderer font roles with mockup system fonts. This is a corrected direction for user comparison, not approved
geometry or a commission for C. No new client launch, painting, render batch or
art import; required future native input/lifetime/layout acceptance stays open. Background inspection alone is not original GUI testing.
Integrated Hero screen and separate Spellbook/Orders remain required; school art
is NOT rejected. Existing ownership and native-execution restrictions persist.

HISTORICAL ONLY — REVISION B bounded integration-readiness (NOT approval): read actual external
`HoMM3-art/output/hero-orders-ui-20260912-b/README.md` and parsed its full
`asset-manifest.json` (98 clean candidates). Existing six command descriptors
`NH_{charge,holdTheLine,advance,aggressive,defensive,cancel}_button.json` all
reference exactly B's64x64 normal/pressed/disabled/highlighted filenames at
 group0/frames0..3. These24PNG are a concrete resource-only prototype opportunity;
no descriptor/code rename needed. This is not import or packaging authorization.
Gauntlet `NH_orders_entry` differs from current sealed source2's
`NH_hero_actions_entry`; requires deliberate dedicated descriptor/client binding,
not a blind overwrite. Action80 buttons likewise need dedicated animation binding
instead of global `settingsWindow/button80` replacement. Panel actual files are
`NH_orders_material/base.png`; manifest's historical geometry calls it
`NH_orders_panel.png`. Current opaque procedural painting must be adapted before
material can show.140px command cards fit V2 only, not V1's192px cards. Hero
Skills/Army geometry and12x16 growth-arrow consumer remain provisional. Clean
assets alone are runtime candidates; private portraits/reference ORA layers,
illustrative inconsistent statistics/growth/percentages never become live data.
No new import, render batch, native execution, license/final-art acceptance or
source branch created. Existing blocked routes and source2 freeze preserved.

CURRENT COORDINATION TOPOLOGY: use name targets `HoMM3:Runtime`,
`HoMM3:Frontend`, `HoMM3:Build`, `HoMM3:Content`, `HoMM3:Artist`.
Dispatcher is `HoMM3:Dispatcher`, but do not inject messages into its user chat.
Old NewHorizons aliases are removed; existing window identities/processes/
conversations persist. Future wakes use HoMM3 names. No agent/model/goal reset,
GUI/build permission or resumption of safety-blocked execution is implied.

LATEST USER AUTHORIZATION: focused SIX-SCHOOL private art previews, independently
of QS/Charge/Focus/Hero compilation. Actual Frontend overlay ready at
`research/six-school-art-intake1/identity.json` SHA
`db519dd01ec5753d0cd6e720a75aa1e878facfd9e15baab15eb6e57618acaa5a`:
96new-familyPNG+12descriptors; full144PNG/18descriptor map. All six schoolBorders
must point to `NH_<school>_spellBorders.json` (light/nature/sorcery/havoc/shadow/chaos),
frames0none/1basic/2advanced/3expert. Existing48SorceryLightPNG+6descriptors unchanged
on bothbases.114consumer-mappedPNG after sixconfigchanges;30emblem/buttonPNG remain
UNBOUND. Both ShadowBasic initial/correction prompt pins retained; private-template/
alpha/edge/provider/rights qualifications preserved. No rootconfig edits byFrontend.

Build ACTUALLY produced both resource-only bundles in10.45s, result read:
`build/six-school-preview-result1.json`; Linux archive
`build/six-school-preview-linux1/New-Horizons-Six-School-Preview-Linux-x86_64.tar.gz`,
Windows `build/six-school-preview-windows1/New-Horizons-Six-School-Preview-Windows-x64.zip`.
144PNG/18descriptors/all6bindings reported, oldbinaries andSorceryLight unchanged,
freshsix-school profile markers inspected, no helper executed. Content changed-
package gate pending. Frontend found actual BOTH README bodies retain stale48/6/
10unbound/54 andtwo-school visualtest/currenttitles below six-school heading;
sent Build exactreplacement request before delivery. CORRECTED archive2 nowbuilt,
actual `build/six-school-preview-result2.json` andWindows2 README read:144/18=162,
114mapped/30unbound/all6retets, obsoleteactive48/54 copy removed. Current Linux:
`build/six-school-preview-linux2/New-Horizons-Six-School-Preview-Linux-x86_64.tar.gz`
SHA `aa216cd7cbff56d50e4d723fa0332c42d04065ac4f00959417a2d6c1156f280c`;
Windows `build/six-school-preview-windows2/New-Horizons-Six-School-Preview-Windows-x64.zip`
SHA `ce415ac269ed9bfa989b1da6312261fa7cd8181c5d79204ea25af0a787eca723`.
Build actualEXIT0/10.47s, archive1 preserved, resources/helpers/binaries unchanged
from1. Content final2 package gate now PASS; actual
`testing/four-school-intake-independent1/package2-readback.json` read: archive/stage/
sums/deltas/sourcecompanions match, all6effectiveborder bindings,144PNG/18descriptors,
114mapped/30unbound,54SorceryLight files and originaltwo-school archives preserved,
bothShadowBasic prompts bound. No remaining package/binding defect identified.
This is NOT nativefit/finalart/publicrights/Windowsgameplay acceptance; no helper/
client executed. Corrected private previews are ready for user visual review.
UIcommission geometry supplied: Hero800x600 draft; Orders/selector640x500 (notold520),
gauntlet/book48x36, reusablebuttons80x32, V2 four140px cards/V1 three192px cards.
External art-only Codex commission does not transfer productcode ownership.

PRIORITY CORRECTION (#448): stop expanding uncompiled UI branches and audit/proposal
infrastructure. No new Hero implementation branch was created; current operation
ended with source inspection only. Concrete user-decision preview:
`build/new-horizons-linux/research/combat-focus-layout-source2/contact-source.png`
(Orders/Focus schematic, NOT native/final art). Earlier Hero sketch preview remains
`research/hero-orders-redesign-source1/hero-overview-wireframe.png`.
Build asked to use an ALREADY permitted resource-only route for reviewed QS/QL
resources now, clearly Charge50-pending, or report the exact blocking contract/action.
No fresh compile, new controller scaffolding, safety bypass or frozen-profile change
requested. Current Linux client proposal is planning-only, not execution admission.
Actual local search still found no Charge-immunity output in modImages/external art
output. Dispatcher must dispatch the existing50px art request to an image-capable
session; request text is not an asset. Full goal remains open, but deferred routes
must not trigger further speculative source/audit trees.

Latest FULL Focus target is now source4, not source3/55 below. Personally verified
`build/focus-fire-runtime-source4/identity.json` SHA
`4fcd75aad49ecd94db4e93f8cd953aebbb8b41a2b4a9ec06b8701ecaf1214b00`:
51 member pins,27 root preimages,9 absent paths,36 source bodies; enumerated64
source cases. REQUIRED filter `*FocusFire*:LegacyCommandAllocationTest.*`; Focus-only
matches63 and misses the legacy allocation control. Both Frontend declaration
headers identical to source3. Receipt `research/focus-fire-source4-frontend-receipt.json`.
Pin/case intake is NOT full semantic/native approval. Subsequently read all247 lines
of allocation1 diff and verified both proposed bodies exactlymatch source4; narrow
allocator correction SOURCE PASS at `research/focus-fire-allocation-frontend-readback1.json`.
Dense-set admission catches[0,1,3], permits shuffled dense IDs, next-ID-only ADD/cap
and retainedghosts preserve identity without renumbering. Five explicit sourceMODEL
rows; reader omission is injected after binary decoding, not a naturally produced
save. Aging4/missing-battle2 follow-ups now read completely andexact-match source4:
`research/focus-fire-aging-context-frontend-{review1.md,readback1.json}`. Command-only
value-snapshot aging/ghost handling/current queue IDs and missing-context guard are
narrow SOURCE corrections, not observed native scoring, retirement/rollback or
full save/AI acceptance. Fresh Build compile/registration and native gates remain.

Separate Extras correction delivered: `research/extras-quick-exchange-source1/`
identity `22d7bb732c4decec4af4d682f43b4a7edf30ae958a24949e98249927ab254a87`.
Confirmed actual callbacks/controllers; corrected exactly2 per-slot arrow blocks to
SOURCE hero ownership. Old8 MODEL rows/four mismatches retained; fixed8/8 andtwo
reverted direction mutants pass, root/controller pins unchanged. Content reports
independent6-member/exact-reconstruction PASS in
`testing/extras-consumers-independent2/correction-readback.json`. No root/asset/
native/rights/allied-GUI acceptance or focused-repair mixing. TRADEQE still activates
whole companion layout, never import only its background. Read separate
`testing/extras-consumers-independent2/SCHOOL-ICON-COVERAGE.md`: four legacy symbolic
school subtype icon mappings do NOT establish six-NH-school coverage or numeric
Air->Sorcery aliasing. Actual subtype/value/default fallback and spell-specific
immunity route need separate saved-subtype/rights/native controls; no new bug or
first-Charge50 gate inferred.

Mutable combat work5 adds observed phase/shared-budget messages and view-only active
Order/Doctrine borders, clearing borders on inactive/expired context. Actual OR of
heroCommandUsed/castSpells, never mana as Orders budget. FEEDBACK5.md +five source
mutants/four-row model andexisting15 controls pass; geometry unchanged fromwork4.
Content work5 independent scoped PASS at `testing/orders-feedback5-independent1/readback.json`:
only refresh changed versuswork4, sixroots/otherbodies/layout/schematic unchanged;
actual OR/phase/border APIs reviewed, not native or source6 approval.
Content's scoped work4 readback `testing/orders-layout4-independent1/readback.json`
binds26members/six roots and reviews actual helper/manifest/schematic, not native
fonts/hits/lifetime or source5. Dispatcher/user layout/art approval explicitly still
needed before expensive generation; no commission or charter transfer.

CURRENT SEALED combat client successor is `research/combat-entry-split-source2/identity.json`
SHA `d0752e0e2cd24b3e0f6778e0e084dc889f220d3f630c1d181f5a0db0d75229de`:
22 members/eightexactwork7 bodies/sixunchangedroots/twoabsentnewpaths, Runtime4 pair.
Content sealed PIN PASS `testing/combat-entry-split-independent2/readback.json`;
source6 routing and source7 copy reviews remain scoped, not C++/native acceptance.
Work7 corrects generic 'selecting is free' ambiguity: ordinary icons issue immediately,
Focus selection is free and requires Confirm; accepted commands share the budget.
Invalid modal says no command sent HERE, not global unspent. OnlytwoCPP copy/readback
changes, threeadditional copy mutants pass; previous24/15/5/9 checks retained.

Personally viewed `research/combat-focus-layout-source1/contact-source.png` and
corrected `research/combat-focus-layout-source2/orders-v2-source.png`. Initialcopy
finding preserved in source1/REVIEW.md. Corrected source2 has editable drawing code,
PNGschematics, ASSET_MANIFEST_DRAFT.json and NATIVE-GATES.md. Content personally
viewed correctedcontact too. Placeholder data/Pillowfonts/flatmaterials NOTnative,
finalpaint or generation. Exactproposed80x32 original reusableactionbutton nowlisted;
currentcoreDiBoxBck-derived control remains qualified. User approval stillpending.

Build private compile-PLANNING proposal read at
`build/combat-private-compile-intent1/proposal.json`: verifiesd0752e, sixrootANDGit168
preimages, Runtime4/registrationb50; distinctCLIENTON SDL2/PCHOFF lane. NewCPP/header
registration, B/localization/art andfreshdependency/search/controller admission
remain. No privateapplication/configure/compile/GUI permission from this receipt;
no headless64, focusedQS/QL/Charge50 or frozenpreview coupling.

Independent Hero preparation: `research/hero-main-lifecycle-source1.md` traces
artifact-holder destructor/TRANSITION_POS/request boundaries. Newtabs mustretain
one holder, not trigger putBack/erase by recreation; allow Equipmentreturn even
with late pickup. Picked-state query is NOT an in-flight request acknowledgement.
No newHeroCPP or observednativeartifactloss claim yet; implementation next.

Historical private combat work6 predecessor: `research/combat-entry-split-work6/`
STATUS6.md/checkpoint6 SHA `a02648c560abaf48143ee2565cd1b2665d6ef336076229cc3e0aed14c37889b3`.
Runtime agreement read: `research/focus-fire-modal-runtime-agreement1.md`, private
source4 API only. Eight client bodies: sixoldrootpreimages unchanged, new
FocusFireTargetWindow.{h,cpp} absent fromroot. New CPP requires Build registration.
Capability-gated fourthOrder plus640x500/8-row modal, immutable value-ID selection,
separatefresh Confirm, weakbattle/ID/round/side/optionalplayer/controller guards,
localclosed/submitted latches, freeCancel/Back and no rawasyncunitptr/actionhex.
Synchronouscount/name/currentrow-column; retainedinactive mark/cohort/round/premium
readback. Existing core80x32 generated buttons are DiBoxBck-derived placeholders,
NOT original final artwork. V1 three-card bounds preserved; v2 uses140px cards.
24modal+15entry+5feedback+9spell textualmutants pass, declaredgeometry6 model only.
OptionalPlayer typing correction and substring-checker surviving-mutant RED retained;
no compiler/native claim. Content source6 review requested, no GUI/build/firstrepair
gate. Work4 schematic/manifest remains v1, not newv2/finalart approval. Full Hero,
originalart/native/persistence/platform requirements still open.

Content four-school TECH intake now PASS at
`testing/four-school-intake-independent1/{summary.json,visual-note.json}`; read status/
qualification and visual note. Their96-output/28-master-pair/12-descriptor audit is
separate from Frontend's earlier96 checks. Prompt/generation records hashed, not
independent tool/model verification. No individual spell-art, final user/public-rights/
import/runtime claim; all alpha/clipped-edge/visual advisories retained. Content's
`provenance-readback.json` now reports28 local chains consistent; inspected status/
qualification. Shadow Basic selectedattempt2 points to `correction-prompt.txt`, while
manifest `basic/prompt.txt` is INITIAL. Keep BOTH prompt pins in every intake notice;
no new repaint requested. Local provenance consistency is not provider invocation,
attempt-budget/cost, model or rights proof.

Current full-graph follow-ups sent to Runtime (SOURCE, not native failures):
`research/focus-fire-ai-order-expiry-source-{red.md,pins.json}` traces candidate
N_TURNS1 Orders through hypothetical nextRound: Focus map clears but legacy Order
bonuses remain (NTurns TODO; CUnitState only resets flags), potentially skewing
multi-round AI comparisons. This is a pre-existing projection gap, not actual
battle expiry or a regression blamed on source3. Doctrine/general spell semantics
must stay intact in any owner fix; source/native regression requested.
`research/focus-fire-save-allocation-source-{followup.md,pins.json}` adds allocator
analysis beyond earlier narrow batch4 ownership review: unique/in-range IDs[0,1,3]
pass identity predicate but nextUnitId=3 collides; traced Lua addUnit/ADD append path.
Requested owner review of allocator-safe v2 admission/allocation and load-then-spawn
oracle, preserving legacy policy. No naturally produced save or native failure
claimed; previous narrow positive readbacks remain scoped, not full-graph approval.

Content independent SOURCE review now PASS for sealed27d566 source1; actual
`testing/combat-entry-split-independent1/REVIEW.md` read. No narrow routing defect,
not compile/GUI. Separate mutable `research/combat-entry-split-work4/STATUS.md`
and checkpoint4 implement Orders-only640x500 code-material layout, three Orders/
two Doctrines, live header/effects/footer and native64px cancel548,416. Original
combined520 mode preserved, no crop/replacement of its backdrop. Geometry script
checks declared rectangles plus24 actual64x64RGBA descriptor frames;15+9 existing
source controls pass but do not certify new layout. Personally viewed Pillow
`panel-source-schematic.png`, NOT native rendering. `ART_LAYOUT_MANIFEST_DRAFT.json`
now records48x36 pointing-gauntlet/640x500 panel roles and live-text/hit regions,
new separate panel basename/no-baked-grid constraint. No art dispatched/final user
approval, source4 integration or first-repair gate. Source1 remains unchanged.

Historical sealed functional v1 combat SOURCE offer: `research/combat-entry-split-source1/`
identity SHA `27d566bad60c0d8c5b14e3061ae523b79c0b412fecefda1462483bff79a276dd`,
12 members/6 client bodies. Content independent source review requested, NOT GUI or
build/root approval. Source3 switches work2's direct key callback to canonical
loadButtonHotkey/addWidget registration with empty-callback button construction;
active assigned button suppresses window dispatch.15 textual mutants include dead
positive tails and duplicate callback insertion; existing9 chooser guard also pass.
Temporary48px entry/640x520 back remain explicit nonfinal art; B config/localization
pairing still Build-owned/proposed only. Prior work1/2/3/history preserved.

Savebatch4 narrow source review/pins now recorded in
`research/focus-fire-savebatch4-frontend-{review.md,readback.json}`:5 proposals,
4 preimages and1 new path verified. Read full diff and actual CStack ctor/serializer/
postDeserialize. Descriptor temporary values are copied; base resolves from army+
slot after loading. Owner-positive and null-before-binding look coherent. No new
narrow defect found, but no combined36-body/59-case, native or disk-save approval.
Source3/55 remains current pending consolidated successor and remaining graph review.

Previous combat source checkpoint is `research/combat-entry-split-work2/STATUS.md`
and checkpoint2.json: six private client bodies, appended BATTLE_OPEN_ORDERS/string
battleOpenOrders, one window key callback (manual button has no assigned key),
shared key/button blocking and tactics block-before-disable/enable. Exact old
shortcut values preserved. B proposed only; Build-owned config/localization pairing
not written or requested as a repair gate. Read modal deactivation and both SDL
printable-text suppression paths; native held-key/chat/modal/lifetime still pending.
10 textual mutants plus existing9-mutant chooser guard pass;6 root pins unchanged.
Initial checker ValueError on missing-token mutant preserved/corrected, not C++ RED.
Temporary art/geometry qualifications below remain; work1 preserved, no compile/root.

Previous combat implementation checkpoint: `research/combat-entry-split-work1/`
contains4 copied client bodies, ROOT-BASE/checkpoint1, STATUS and read-only source
checks. Private v1 prototype implements direct Spellbook, independently admitted
Orders entry,349px console/51px arrow shift, and Orders-only chooser with null-spell
refresh guards. No root integration/compile/native or final-art claim; old48px
entry/640x520 backdrop are explicit placeholders, B unbound.7 textual mutants
rejected and4 root preimages unchanged. This is actual private source progress,
not finished UI; no FocusFire API calls and no convenience/profile mixing.

Full FocusFire3 review found SOURCE RED in2 callback seams: battleMatchOwner uses
CURRENT attacker but INITIAL defender owner (unchanged Essentials helper), so its
hostile splash prediction differs from authority's current/current comparison and
premium can remain on a currently friendly target despite inactive mark readback.
`research/focus-fire-source3-controller-red.{md,json}` pins source/truth table, no
native failure claim. Runtime confirmed/preserved and reports narrow immutable
`build/focus-fire-controller-source1` correcting2 seams plus strengthened tests,
pending combined savebatch4. Narrow correction now personally read and pinned in
`research/focus-fire-controller-source1-readback.json`: exact2 callback replacements,
2 strengthened existing cases and unchanged Essentials verified. This closes the
narrow SOURCE readback only, not combined/save/native acceptance; Source3/55 remains
current. Do not globally change ordinary shot/owner rules.

Current remaining-school intake: `research/four-school-art-readback1/REVIEW.md`
and readback.json record personally viewed six-school/all96 sheets, four family
REVIEW docs and independent96 PNG SHA/dim/RGBA checks plus four header top28 alpha
clearances. All24-per-family role counts pass. Content's owned-Light readiness is
`testing/light-preview-intake-independent1/FOUR-SCHOOL-READINESS.md`; their note
correctly attributes Dispatcher checks rather than claiming their own full repeat.
Shadow32 darkness, narrow Havoc emblem and glossy pink Chaos are visual advisories,
not rejection/final user approval. 144 total school-family review images is NOT
individual spell artwork. Native source alpha252/253, clipped tips, private template
rights and unadmitted new border bindings remain qualified. No import/build/GUI,
charter change or additional focused-repair gate; existing previews frozen.

Current parallel source checkpoint: `research/hero-orders-redesign-source1/` contains
PLAN.md, source-snapshot, four SVG/PNG schematic wireframes and private HEADER-only
resource evidence. Viewed both user sketches and rendered overview diagram. Measured
HeroScr3/4=672x586, ICM005=48x36 in all4 frames, ComSlide=18x17; no pixels exported
from purchaser archives or mount-precedence/native proof. Proposed new main Hero
800x600 integrates Overview/Skills-Masteries/Equipment/Army; equipment needs native
382px height so overview army strip is hidden on that tab rather than scaling slots.
Combat proposal Orders595,560 at48x36, originalBook646, console349wide/arrows574.
O is globalOptions; B is only a distinct battle-key proposal pending modal gating.
Real saved data/action map and explicit absent/legacy cases documented. Hero lower
control bounds, font/flow/input review and final art regions remain un-frozen. No
implementation or art commission approved by these diagrams, and no candidate mix.
Successor CONTROL_GEOMETRY2.md/control-geometry2.json now check measured footer:
HSBTNS52x36, arrows22x46, formation/tactics54x32; generated Commander92x38 and
Backpack52x36 across four states. Footer y496..570 clears status572; all7 army
slots disjoint. Artifact union is279x382 (left arrow x20, gesture x21+278), not
initial278 reservation. All19 worn+5 backpack+2 arrow rectangles checked disjoint;
gesture overlap intentional. Three model challenges reject old width, generic
Commander and close/status overlap assumptions. Initial diagrams retained; no
native inference. Hero switcher's existing pop/recreate path needs explicit
carried-artifact/current-context handling in integration. Continue combat split
and latest FocusFire3 source review independently; geometry/model is not completion.

Focused convenience: inspected Content's independent responsive3 source/art report
(56pins,16 decoded RGBA frames,36outputs/8inputs, exact vector transforms). No native
or combined gate. Explicit charge dependency clarified to Build/Content: the
single50px request is NOT dispatched and no foreground exists here. Dispatcher must
route CHARGE_IMMUNITY_ART_REQUEST.md to an actually image-capable homm3-art session;
Frontend has no generation tool and Artist remains Sorcery-only. No source-path-as-
asset claim; larger UI/catalog work is NOT a gate on the focused repair.

Latest checkpoint: responsive SOURCE slice is SEALED at
`research/convenience-responsive-source3/identity.json`, SHA
ca018dfb56082a1655c05e618f45cb1c60b47d5e505ad6eb6af001bcbd5e21cd (56 member pins).
Recipe3 remains10c5b791; Build agreed its adaptations and readback report records
156 paired-base samples using Frontend's model, not a renderer.665 gets a259px
list only;666+ retains260; compact lower filler starts667. Expanded geometry stays
unchanged. Seven read-only tests (5 model+2 art),78 geometry scenarios/14 negative
controls;36 fitted-art bodies reproduced. Original recipe2 negative665 and initial
model hidden-world-background RED preserved. Matching charge art/combined gate and
native journey remain pending. No merged widget/root/stage/profile write.

Read `docs/NH_HERO_ORDERS_UI_REDESIGN.md` and viewed BOTH actual private sketches.
Larger main-Hero integration and separate combat Spellbook/Orders are now explicit
next source/wireframe work, not additions to the focused convenience candidate.
Do not commission gauntlet/panel until actual toolbar/canvas/text regions are frozen;
sketch free points/Replace Skill/numbers and experimental castellan rules are not
activated. Existing shared hero-action budget and independent bookless Orders/spell
admission must survive the split.

Latest Focus Fire combined-review target is now source3, NOT source1/2. Receipt
`research/focus-fire-source3-frontend-receipt.json`: identitycebfab755b597790595ae5cf6d3d47294b14469edf815c59d4dd8ea1e8244306,
45 member pins; exactly CBattleInfoCallback.cpp/FocusFireAITest.cpp changed from2.
Source2 raw API.md-equality RED was just version/count metadata, preserved separately;
no API-document byte equality claimed for3.55 cases remain SOURCE only. Full code
review not approved; no UI wiring/compile/native run or convenience mixing.

Prior checkpoints below remain evidence, not latest intake authority:
Content is sole additional upstream fetch owner; no new fetched
files from Frontend (one earlier URL attempt404 only). Retained reference comparison
`live-convenience-repair1/parent-comparison.json` exposes source-only negative filler
at logical865..888 in upstream expanded routing. Build approved the OPERATION of a
build-time named-node merge, not any geometry or stage execution. `recipe2.json`
is a REVIEW-ONLY three-target proposal with paired raw Linux413/Windowsd90 base
hashes, canonical old-subtree hashes, exact replacements and reverse-equality rules.
900+ expanded uses retained32px normal sprites centered in64px column, own wide
QS516/QL548; native list counts preserved and lower fillers split to avoid painting
over controls. Compact retains NextHero before QS/QL. Expanded tail0/32 explicitly
empty pending Revisit/Search image review. These adaptations need review; not sealed,
not tested by old layout1 controls, and not a complete Extras integration claim.
`CHARGE_IMMUNITY_ART_REQUEST.md` supplies the exact50px role and semantics for actual
image-capable generation; no tool execution/native foreground claimed. Button-fit
art remains retained. Next: recipe2 geometry/reverse-delta negatives and cross-owner
agreement, then matching original charge-art intake and a sealed combined offer.

Separate Focus Fire wake received: sealed source1 identity0ec088133a7a8bb896e712df9dfead543cd7cd7fa20beccc2e32feefa56e310a;
CONTRACT/API read and all42 member pins (34 bodies) verified. Receipt at
`research/focus-fire-source1-frontend-receipt.json`, NOT combined code approval.
No root/UI wiring/native run. Full sealed implementation review remains queued
behind the current user-priority convenience repair.

Read `docs/NH_EXTRAS_INTEGRATION.md`; its coherent component scope supersedes a
single-icon-only interpretation. User reports smooth native Linux movement, not
full acceptance. User/profile may remain live: no hotpatch, launch or competing GUI.
Pikeman/Halberdier are CHARGE_IMMUNITY, not intrinsic FIRST_STRIKE. Correct the
initial hypothesis; Build mapping name agreed `NH_status_chargeImmunity_50`.
No new status image/mechanics/creature/description change yet. Content independently
bound the actual413 fallback chain and staged data in testing/two-school-user-feedback1.

WIP `research/live-convenience-repair1/`: retained413 consumer sources/findings;
original NH button-art fitting script yields16 SVG/16 native32x32 or64x32 RGBA PNGs
and4 descriptors, eight input SVGs unchanged. Native contact viewed; no Extras
pixels/new concept generation, user/style/runtime acceptance not inferred. Important:
413 buildMapButton uses image-native size, not JSON area width/height.

`layout1/` is an UNSEALED native-minimal comparison, NOT accepted integration:
three exclusive logical-height regimes <=664/665..864/>864, NextHero retained,
QS/QL below native controls, EndTurn/filler moved to avoid overlap. It does not
reproduce the entire Extras tall-toolbar redesign and omits buttons <=664 (Extras
also does so; F8/F9 unchanged).2 static tests cover7 heights+10 negative mutations,
0.009s; not GUI proof. Build was told not to ingest the full-file overlay proposal
under the new no-whole-widget-overwrite contract. Next resolve targeted pinned-base
container merge and precise accepted adaptive behavior with Build; inventory every
Extras component/dependency/rights exception with Content, not a silent subset.
Retain this comparison and original top171 overlay evidence. No root config,
protected stage/profile, old school art or status icon was changed.

## Fresh413 full-book fixture: bounded SOURCE fit review

`research/two-school-fullbook-source-review1/REVIEW.md` binds the supplied map
SHA56d9a86d to shipped413 source and actual Linux2 inline/config magic. Expected
Basic Light/Advanced Sorcery, not every rank. Static69-common counts: Light12
combat/0 adventure; Sorcery10/6. Small school first-page capacity10 means Light
can show page2/header absence but Sorcery cannot; large capacity22 means neither
has page2. All combat59 gives5small/3large pages, not school-header coverage.
Six-school compact68x51 requires small mode; staged schema defaults large=true,
which keeps80x60. Starting effective new-family borders cover Light1/Sorcery2,
not0/3. Full counts, source pins and limitations retained. No fixture change,
profile creation, native parser, GUI or new admission. Fresh runtime/Xvfb/input
closure and retained-ownership adapter remain execution dependencies, NOT blockers
to the already-delivered private archives.

## Compiled spell-UI candidate168217: local scoped intake, CRLF qualification

Actual Windows package is at build/spell-ui-windows-audit1/
New-Horizons-Windows-x64-1682170557f3. Read its BUILD-IDENTITY/source/run/backend
(SDL3); source companion hash7f6ed91d matches. Four owned archived source bodies
initially failed raw LF pin comparison; all four are EXACT reviewed-LF→CRLF-only
transforms, not code edits. Both raw hashes and preserved RED are recorded in
`research/spell-ui-168217-source-bytes-red.json`; scoped qualified PASS in
`research/spell-ui-168217-frontend-intake1.json` also verifies two primary PE sums.
Do not describe this as raw source equality or full package/native audit. Build
reports1211-file/1210-sum producer gate and85 packaging regressions. Content's
`testing/windows-168217-audit/final-summary.json` now records independent full STATIC
package PASS, not gameplay. Frontend inspected it and verified all21 report pins;
`research/spell-ui-168217-independent-gate-readback1.json` retains this readback,
not a rerun. Scope includes26 AMD64 images,6155 imports,945 resource comparisons,
4717 source files (4093 CRLF-only),24 unchanged413 vendor bodies,113700 dependency
records and227 notices; three current CRTs separately bound. Preserve120 Unix
exec-mode differences, source-path/legacy alias exceptions, conditional licensing,
and the inspector REST-key RED. ENABLE_TEST OFF:85 Python packaging regressions
are not native C++ tests. No public-release authority is inferred.
This candidate does not replace either frozen art preview;
actual normal/cancel/stale/defender-only/no-hero/lifetime gates remain open.
Copied only the four independently raw-hash-checked CRLF source members into
`research/spell-ui-168217-archived-source-controls1/` and ran the two archived
Python checkers against those archived C++ bodies:9+5 source mutants rejected.
This verifies the source-export/checker path, not the client or widget runtime.

## Experimental documents read — no implementation scope change

After two-school package delivery passed, read both supplied Reconstruction
Experimental documents fully, preserving originals. Design-only frontend review:
`build/new-horizons-linux/research/castellan-caravan-frontend-design-review1.md`.
Keep current soft Leadership, single-currentHero combat API and existing town rules
unchanged. Mandatory local commander and single-expeditionary office are separable;
no autonomous town capacity may be added to later castellan reservations. Absence,
replacement/succession/progression and multi-commander attribution remain unresolved;
do not invent caravan loss deadlines or duplicate command budgets. No code, saves,
preview scope or defaults changed. Actual implementation requires a later decision.

## Current Linux successor2 — metadata-only correction verified

Content found Linux1 inherited identity0555 contradicted actual launcher0755;
Linux1/9abd and its RED remain preserved, not current delivery. Use:
`build/two-school-preview-linux2/New-Horizons-Two-School-Preview-Linux-x86_64.tar.gz`
18,741,324 bytes, SHAb990ddf9b3b538209e5d64693b4949fdba3a139a6d970a2654a7b91acf14cdbc.
Frontend personally hashed BOTH Linux archives and streamed/compared all1175 member
bodies/modes: only BUILD-IDENTITY.json and SHA256SUMS bodies changed; all other
bodies/modes unchanged. New entrypoint_modes match actual archive(client0555,
wrapper/launcher0755); old modes are explicitly base_entrypoint_modes. Report:
`research/two-school-linux2-frontend-readback.json`. No extraction/stage writes/run.
Windows1/bdfe remains the paired package. Inspected Content's final
`testing/two-school-final-independent1/combined-summary.json`:
BOTH_PRIVATE_PREVIEW_PACKAGES_PASS_NOT_GAMEPLAY; all1175 Linux2/1225 Windows1
members, identical54 art files, exact metadata repair, preserved predecessors and
source-companion/permission checks reported complete. Both current packages are
ready for private user delivery. No engine/art/helper change, graphical acceptance,
cross-save equivalence or full redesign completion follows from this package gate.
Any new Content Linux GUI needs its own valid fresh handoff.

## Historical Linux1 / current Windows1 archive checkpoint

- Linux: `build/two-school-preview-linux1/New-Horizons-Two-School-Preview-Linux-x86_64.tar.gz`,18,741,288 bytes;
  SHA9abd47073590df1ee6e524c15a6250cbdf0fcdb027c5ba28cc9fffef0ccfe62d.
- Windows: `build/two-school-preview-windows1/New-Horizons-Two-School-Preview-Windows-x64.zip`,25,458,090 bytes;
  SHAbdfe4e4e1acacfae6c8fe249dbb6aaecc6dce2d455fcc926157c79c014cba4fb.

Personally hashed both complete archives and compared59 Linux/60 Windows selected
archived members with the frozen stages (54 art/descriptor files, helpers/config/
identity/README); Linux scripts retain0755. Report:
`research/two-school-final-archive-frontend1.json`. Both READMEs read completely:
Linux ./Play-New-Horizons.sh --assets '/installed/Complete' with native system
libraries/links and HOME-isolated profile; Windows Play-New-Horizons.cmd copies
licensed assets into its separate LOCALAPPDATA profile. No manual art/config edits.

Build reports full1175 Linux member hashes/modes and1225 Windows CRC/member hashes
passed; those are separate from Frontend's selected-member readback. Two different
unchanged engine bases (Linux413, Windowsd90), no cross-save parity claim. Both
provide identical48 images+6descriptors;10 emblem/buttons remain unbound. No new
native/GUI screens or final appearance approval; no public redistribution clearance.
Old Sorcery-only package/profile are unchanged. Await independent final Content
gate and actual user/guarded visual feedback; full redesign remains incomplete.

## New priority: two-school / two-platform preview payload ready

Read ignored two-school-dual-platform-preview-request.md. Delivered actual
`build/new-horizons-linux/research/two-school-preview-images1/Images`:48 exact final
PNGs +6 descriptors for Sorcery/Light; identity.json and HANDOFF.md supplied to Build
and Content. Personally verified48 manifest SHA/IHDR RGBA8/dimensions, exact6 frame
orders/references, current24 skill paths and both header/bookmark paths. All27
Sorcery files match the previous offer; frozen Sorcery-only ZIP remains unchanged.

Both border bindings require NH_<school>_spellBorders.json in the chosen stages;
existing singular bookmark/button descriptor names are preserved. Only two school
border fields may change, not unrelated dirty config/rules. Both platforms need
new isolated profiles; Linux must use an actual native Linux binary/launcher.
Build selected Windows audited d90 and native Linux public413 (different engine
identities, explicitly not parity). New stages are build/two-school-preview-windows1/
New-Horizons-Two-School-Preview and build/two-school-preview-linux1/
New-Horizons-Two-School-Preview. Delivered actual three-script private offer at
research/two-school-preview-helpers1: Windows9150cd22 (four token changes), Linux
launcherf1e7eeb6 (distinct preview marker only), wrapper2040dc25 (default isolated
XDG/HOME profile and absolute-base check). Full source read, reverse-change checks
and bash -n passed; none executed. Windows five dirs must use matching
HeroesIII-NewHorizons-TwoSchoolPreview1. Linux still links assets, Windows copies;
manual packaged launcher is not a newly certified Tester harness. Await actual
paired stages/freeze for audit; neither final bundle is claimed complete yet.

Policy-aligned successor `research/two-school-preview-helpers2` now supersedes
helper1's Linux defaults: wrapper5854f165 uses exactly
$HOME/.local/share/new-horizons-two-school-preview1; launcher048d27c4 uses marker
'New Horizons two-school preview profile v1'. Windows9150cd22 is unchanged.
Old offer preserved. Source reverse-byte and Bash syntax checks pass, no execution.
`research/two-school-stage-consumers1.json` confirms both actual stage mod hashes
(Windows3d153a62/Linuxefa9ff64), each whole JSON equal to its own base except the
two border pointers, all54 file pins and school/skill/descriptor reference closure.
This does not yet assert helper2 copied/frozen or either package's native behavior.

Actually viewed Light native UI and Light-versus-Sorcery rank/size sheets: distinct
gold/ivory versus blue presentation, including32px and compact bookmarks. Static
viewing is not final artistic or engine-fit approval. Ten combined emblem/button
images are provisioned but unbound to school-specific book widgets. Private use
only; no public/template rights inferred. Do not wait for Focus Fire/other schools.

## Private Sorcery preview ZIP produced — no gameplay claim

Actual local package:
`build/sorcery-art-preview-windows1/New-Horizons-Sorcery-Preview-Windows-x64.zip`
(25,316,780 bytes), SHA256
`3f1c9a8d6f14575c8843007d4058bd5b90099283c0346b732e56b7b567ea2777`.
Build zip-verification reports1220 CRC/member-hash PASS. Frontend personally hashed
that ZIP and compared32 archived helper/config/identity/readme/asset/descriptor
members byte-for-byte with the frozen stage; not an independent1220-file replay.
Evidence: `research/sorcery-preview-final-frontend-audit1.json` and
`research/sorcery-preview-zip-frontend1.json` under the Linux build.

Final helper8f50307d is now actually paired with the five preview dirs. Extract
into a NEW folder on Windows and use Play-New-Horizons.cmd; select legitimate
Complete assets when prompted. No manual art/config editing, old-profile migration,
admin elevation or build tools required. Separate SorceryPreview profile needs its
own asset-copy space. BASE-* records are historical; current README/identity describe
the overlay. Source/dependency-source companions are alongside the ZIP.

This is the unchanged d90 engine with a private art/config/helper overlay, NOT the
new combat guard fixes or Focus Fire. No native Windows execution, all-state hero
fixture, public redistribution clearance or final user visual approval is claimed.
Five provisioned emblem/button images do not become new visible spellbook widgets.
Read external DELIVERY.txt: this qualification is now explicit without modifying
frozen README. Frontend also actually viewed returned review-ui-native.png,
review-borders-native.png and the staged Expert large image. These show native/
compact bookmark contrast, header art, cumulative corner decoration and chosen
Expert output; static viewing is not engine rendering or final artistic acceptance.
Content final ZIP gate is now inspected at
`testing/sorcery-preview-intake-independent1/final-summary.json`:
PRIVATE_PREVIEW_PACKAGE_PASS_WITH_QUALIFICATIONS, all1220 members/1219 sums/CRC,
allowlisted changes,26 unchanged PE files and both source companions verified.
Content additionally reports regular-file ZIP metadata/no-comment controls passed.
These are independent Content results, not Frontend's32-member subset replay.
The earlier supposed new helper guard was an inspector assumption RED, not a product
failure: its mismatch refusal already existed. Frozen ZIP3f1c is ready for private
user delivery; Windows gameplay, user visuals and full redesign remain unproved.

## Prior preview: staged Windows d90 consumer audit PASS

Build chose the existing audited Windows d90 package, staged privately at
`build/sorcery-art-preview-windows1/New-Horizons-Sorcery-Preview`. Read-only
`research/sorcery-preview-stage-audit1.json` confirms all27 asset/descriptor hashes,
12 configured skill paths, group/frame mappings and only one semantic mod.json
change: /spellSchools/sorcery/schoolBorders. Staged mod SHA25a9e2d6ddba9381b3d41a127681aeed13c3ed9f6c85b37886b88a2207def372.
Five dirs.json fields alone switch to HeroesIII-NewHorizons-SorceryPreview.

Delivered private helper `research/sorcery-preview-helper1/Start-New-Horizons.ps1`,
SHA8f50307dfbe758ba6f6e1c0765b1bcbdf02b933cf1281e7b474f3b7565156466:
exactly four profile/product literal replacements from base475bad4c, reverse-byte
identity and CRLF preserved, no other logic change. Build applies it to stage;
Frontend does not edit the root helper or launch it. This deliberately uses fresh
settings/saves/content instead of adopting the normal user's existing profile.

Separately personally compared staged/base VCMI_client.exe and VCMI_lib.dll hashes:
fd8142296893dcc96afd2ae26a197fe9914e97a6b0d6f7c571f6faf9f8ed8af5 and
b56677c6f305e1438187faa574786cfe2fc3fe98979cd767c97440f5fa987434 respectively.
`research/sorcery-preview-stage-binaries1.json` is only those two PE checks, not a
full dependency audit or native Windows gameplay. Artist reports completed fresh
24-output/7-foreground decoded-alpha/provenance intake891bf281; do not wait for
more Artist production. Await final Build package/helper pairing and Content review.

## Prior preview offer: user-authorized private Sorcery image payload

Read sorcery-art-preview-request.md. Delivered ignored
`build/new-horizons-linux/research/sorcery-preview-images1/`:24 exact returned PNGs
plus3 descriptors, identity and Build handoff. Personally matched all24 manifest
hashes and PNG IHDR RGBA8/dimensions; descriptor frame/reference checks passed.
This is not an independent decoded-alpha/visual pass. Original sources, frozen
candidates and product configuration remain untouched.

Normalized incoming plural bookmark/button JSON filenames to existing singular
NH_sorcery_bookmark.json/NH_sorcery_button.json. New NH_sorcery_spellBorders.json
maps proficiency0..3. Build must apply ONLY the chosen verified stage's Sorcery
schoolBorders SplevA→NH_sorcery_spellBorders.json binding and copy27 files under
Mods/new-horizons/Images, not Content/Images. Do not replace dirty whole config.
Use verified existing binaries; pending C++ fixes/Focus Fire/Light are not gates.

Important coverage: skill/campaign portraits, borders, bookmarks and page0 header
have identified consumers. Current source/config lookup has no specific Sorcery
emblem/button consumer; those five images are provisioned, not claimed visible in
the current book. Its generic All button remains NH_spells_button. No inert-control
or all24-on-one-screen claim. Await exact Build stage for lookup/diff audit, Content
freshly guarded checks and user appearance review. Preview import is authorized;
final style and public selected-file rights are not. No game launched by Frontend.

## Combat fix integration: separate Windows FULL path confirmed

Build proposed the working cloud Windows FULL route for exactly the four files in
spell-ui-resumed-integration1, independent of Linux's current-input hold. Frontend
freshly matched root/offer hashes, reran9+5 structural controls and diff checks, and
confirmed owned commit-ready scope in windows-full-scope-confirmation.json. Required
CMake changes NONE; additional test files NONE beyond the two included manually
run source checkers. No native-test registration or runtime proof is implied.
Build alone owns exact allowlist/commit/push/one FULL run and bounded terminal
monitor. Keep those four inputs stable during integration; no art, helper/config,
Focus Fire, unrelated dirty files or docs added to that scope. Actual compile/run
result remains pending; d90 and the delivered Sorcery ZIP remain frozen.

Inspected local commit1682170557f3e5b58ceca57c86ba7ab13ae45fe3: exactly the four
approved paths and prescribed author/committer identity. Build reports pushed and
Windows FULL34691172003 in progress (preflight_only=false, empty repack), under its
195-minute bounded terminal/error monitor. No second monitor or local build started
by Frontend. Subsequently inspected `build/spell-ui-cloud-source-gate1/terminal-query.json`:
run34691172003 is completed/success on exact1682170557f3e5b58ceca57c86ba7ab13ae45fe3.
This records the Windows FULL terminal result, not native gameplay/publication or
independent package intake. The two-school preview bases stay413/d90 as frozen;
do not silently substitute this newer engine into either completed art archive.

## Session restoration checkpoint — fresh source offer, no lease reuse

Re-read current handoff/Build hold and Runtime Focus Fire STATUS (still unsealed).
Prepared `build/new-horizons-linux/research/spell-ui-resumed-integration1/` with four
exact independent2-pinned inputs, restricted two-C++ diff and explicit integration
handoff. Copied-source9+5 controls pass; reverse patch check passes without applying.
Build owns fresh input validation/compile scheduling; Content owns future normal/
stale/caster/cancel GUI gates. No old process ID, approval or native Windows owner
is assumed. Artwork does not block this gameplay-source integration offer.

## Light art handoff boundary — Dispatcher prompt, Frontend consumer integration

Light uses the same24-role school contract, individual spells separate. Existing
skill resources are NH_lightMagic_{basic,advanced,expert}_{small,medium,large,
scenarioBonus}.png (32x32/44x44/82x93/58x64), confirmed in both skill configuration
and curated mod.json. Current school header/bookmark bindings are NH_light_header.png
and NH_light_bookmark.json; schoolBorders still reuses SplevA. Future original four-
frame78x65 border descriptor requires Build-owned registration, not just PNG intake.
Header/page0/top28, effective-proficiency border frames and bookmark0/1/compact
contracts above apply equally to Light. No new motif, file rename, generation or
ownership assignment is inferred: Dispatcher owns the external prompt; Artist
remains Sorcery-only; Frontend reviews consumer fit and approved UI integration.

User reports24 returned Sorcery outputs including revised Basic/Advanced and gryphon-
claw Expert. This supersedes the earlier pending-generation status only as a REPORT:
Frontend has not inspected returned bytes/placements/rights or approved import.
Artist requested a fresh Build light read-only slot; await exact reviewed intake,
not an assumed external image transport or a request for user technical work.

## Future Focus Fire boundary — no UI implementation yet

Read Runtime's updated `research/runtime-focus-fire-contract1.md`; Frontend review
is `research/focus-fire-frontend-contract-review1.md` (both under the Linux build).
BEGIN(any statically legal target) and CONFIRM(exact battle-unit ID) are separate
read-only queries; actual request uses unit ID + INVALID hex and server validation.
No raw unit pointers across asynchronous boundaries. Retain weak battle context,
value IDs and round checks, no-spend cancellation and inactive-mark readback.

Clarification: all shooters having acted does NOT itself disable BEGIN if the hero
phase/budget remains legal. Static shooting legality is not another activation;
feedback must not promise an extra shot. Issuance cohort is frozen by IDs using
CURRENT controller (`battleGetOwner`), not original unitSide: enemy-origin hypnotized
shooters can join at issue; excluded IDs do not join when control later changes.
Included IDs can lose/regain effective benefit within the round. Full callback,
AI/damage/save source is still pending; the isolated rules component alone cannot
be wired or called integrated. Existing d90/aaed and the two source-only spell UI
repairs remain separate. Await the arranged Runtime API offer, not a new GUI run.

## Current integration dependency — Linux input hold, not source acceptance

Read current NH_BUILD_HANDOFF: Build's Linux hold remains active after the host
upgrade; its inventory reports more than the initial four link-body changes and
explicitly does not establish a new complete closure. Compiler-execution DSOs and
fresh ABI review remain required. The two delivered combat UI repairs are still
source-only; no old loader/compiler fence or Windows artifact admits their Linux
compilation/GUI. Await the arranged Build current-input/integration wake and
Content's separately authorized runtime gates. No pin refresh, install, rollback,
probe or alternative frontend GUI execution is requested.

## Latest checkers checkpoint — normal-route structural gaps repaired

Inspected Content's `testing/spell-ui-source-independent1/summary.json`: five pins
stable,12 original mutants and two historical-source RED controls; independent
normal-route controls exposed that both original checkers accepted a post-guard
unconditional return. No product defect was found in those challenges.

Updated only the two owned Python checkers to reject those mutations. Chooser now
requires the exact post-refusal close/open tail; caster rejects later returns in
its normal targeting route. Successor9+5 in-memory controls PASS. Original checkers
are preserved in `research/spell-ui-source-checkers2/history/`, with successor log
and pins alongside. Initial successor console retained a hardcoded4 count for the
caster's five controls; corrected to derive len(mutants). No C++ change in this
checkpoint. This remains structural coverage, not an execution/reachability proof
for arbitrary mutations. Compilation and all actual normal/stale/defender/refusal
GUI gates remain open.

Inspected successor `testing/spell-ui-source-independent2/summary.json` and personally
rehash-matched its five current source pins. Content reports9+5 producer mutants,
two historical aaed-source REDs and both extra post-guard-return challenges now
rejected. Three C++ context bodies are unchanged from its predecessor. This closes
those two structural-checker gaps only; no independent-control rerun or runtime
acceptance is claimed by this read/hash check.

## Prior control checkpoint — null-safe spell caster (source only)

`BattleActionsController::castThisSpell` previously dereferenced attackingHeroInstance
when selecting the caster, even if only the defending hero existed. It now checks
curInt and uses the existing null-safe `BattleInterface::currentHero()`; no hero
means return BEFORE allocating/changing heroSpellToCast. Existing targeting and
server request routing remain unchanged. This is a source-identified null dereference
risk, not a reproduced graphical crash or broader callback lifetime repair.

`client/tests/check-spell-caster-routing.py`: source contract PASS, four in-memory
missing-guard/unsafe-lookup/early-mutation mutants rejected. Log and exact pins in
`build/new-horizons-linux/research/spell-caster-routing1/`; diff check passed.
No compile/native/GUI performed. Future Build/Content verification must cover an
ordinary attacker caster, defender caster with absent attacking hero, and stale
no-interface/no-hero refusal without modifying targeting state. No rules/CMake,
frozen candidate, helper or asset changes; sole Build integration remains pending.

## Prior control checkpoint — chooser spell activation recheck (source only)

`client/battle/BattleHeroActionWindow.cpp::chooseSpell` now rechecks current turn,
Autofight, tactics, targeting, hero presence and authoritative spell availability
BEFORE closing the chooser. Previously only battle existence was checked there;
button blocking was refresh-time, and BattleWindow's downstream opener did not
repeat the Autofight/tactics guards. Refusal now refreshes and retains the chooser,
consistent with chooseCommand. This is UI stale-state hardening, not a replacement
for server validation or evidence that an illegal cast previously executed.

`client/tests/check-hero-action-spell-routing.py`: old source RED preserved in
`build/new-horizons-linux/research/hero-action-spell-guard1/source-before-red.log`;
new source contract PASS plus8 in-memory guard/return/order mutants rejected in
source-after.log. Diff whitespace check passed. These are structural source checks,
NOT compilation, actual widget execution, lifetime or graphical acceptance.
Build owns future compile/integration; Content owns actual stale-state/normal
spell/cancel usability checks after authorized assembly. No frozen d90/root binary,
profile, rules, CMake or artwork changed; no native build or GUI launched.

## Latest school completeness correction —24 outputs, not20

Read `NH_SCHOOL_ART_COMPLETENESS.md` and inspected current SpellSchoolHandler,
CSpellWindow::SpellArea::setSpell/setSchoolImages and curated mod.json. Sorcery
currently binds schoolBorders="SplevA" (original Air reuse). A future approved
NH_sorcery_spellBorders.json must be registered via schoolBorders; image files
alone cannot replace that binding. Build owns non-Image registration; no live
config, descriptor, art or renderer change is made by this inspection.

Border consumer: CAnimImage at the spell area's native origin, group0, frame
schoolLevel from hero->getSpellSchoolLevel(spell,&whichSchool), with no explicit
scaling. All tab uses whichSchool when valid; a specific tab uses that tab's border
FAMILY but still the spell's effective schoolLevel. Do not claim selected-tab-only
skill rank determines the frame, especially for multi-school spells. Clearing a
spell resets its border. Proficiency0..3 is not a mastery-talent selection.
Reported private original78x65/four-frame corner progression is source-compatible;
Frontend has not independently re-extracted those private border pixels here.

Bookmarks use selected0/unselected1 in group0; selected bookmark is brought to
foreground. Custom header is native CPicture at(117+offL,74+offT), page0 only;
setSchoolImages resets it on later pages. Its160x96/top28-clear art contract is
not enforced by a runtime crop, a fullscreen splash or four proficiency variants.

Correct current full-school inventory:12 skill images +4 transparent border
frames(none/basic/advanced/expert) +2 bookmarks +1 header +1 emblem +4 button
states =24 images, descriptors and individual spells separate. Current approved
DIRECTION/PLANNED12 skill request is unchanged;12 school outputs remain, not8.
Earlier20/remaining8 statements below are historical inventory omissions, not a
scope cap or acceptance. Actual alpha/corners, native/compact readability, multi-
school All/selected behavior, user visuals, rights and Content GUI gates stay open.

## Latest artwork checkpoint — approved process, assets still gated

Read `NH_APPROVED_ART_WORKFLOW.md`: user-approved default is artistic request →
actual art-capable generation of native RGBA → alpha/edge QA → exact native-template
composition → actual user visual review. Artist owns generation intake/compositor;
Frontend owns approved UI integration. No user manual masking/modeling chores,
parallel Sorcery generation, repeated extraction loops or fictional dispatcher
transport. One initial attempt and at most one targeted correction per request.
Spindle foreground953af277 and near-opaque252/253 alpha are the documented process
example, not final motif/family/import/style/rights or named-model approval.
Historical04/background/mask/Blender routes are superseded, not pending decisions.
Future asset work follows the canonical workflow; product UI work remains separate.

Latest artistic direction is now accepted: Basic scroll / Advanced open book /
Expert brass-held orb, with blue aether rather than lightning. Read the complete
Artist request `assets/new-horizons/sorcery-art/requests/sorcery-blue-aether-skill-01.json`;
independently matched SHA4a73526a3f739b049e593b97b29da45dbc0814c95cf88405dac07b4313e9aecb
and all12 resource names against config/newHorizonsSkills.json. Scenario bonus
selection directly uses skill->at(mastery).scenarioBonus in CBonusSelection;
bonusBlank58x64 remains a provisional template/fit/rights choice, not bonusSpell.
This is a PLANNED12 skill-image request with null art/placements/output hashes,
not actual image approval. Eight additional school-UI outputs are explicitly
retained in the manifest; full20 scope stays open. No generation/transport/import
claimed; Artist owns intake after actual external art arrives.

## Spell art consumer follow-up — source dimensions, not mounted evidence

Read `NH_ART_ASSET_SPECIFICATIONS.md`: each request expands to its actual role
family; a representative concept is only a staged gate. A request manifest must
separate role/rank/state/size/resource/template/placement/review status. No new
asset, renaming, import or GUI operation accompanies this source inspection.

- `CSpell::registerIcons` binds iconBook→SPELLS[id], iconEffect→SPELLINT[id+1],
  iconScenarioBonus→SPELLBON[id], iconScroll→SPELLSCR[id], group0. Preserve the
  effect +1 offset; iconImmune is NOT registered in those animations.
- `CSpellWindow::SpellArea` uses native SPELLS frames at the area's origin without
  resizing. Its interaction rectangle is65x78, NOT an image-resize contract;
  labels are centered at x39/y70,82,94. The67x48 book template remains the native
  artwork candidate, not a claim that the hitbox is67x48 or clips the image.
- Mage-guild `CCastleInterface.cpp` scroll constructors use native SPELLSCR frames
  and copy image->pos into the widget; no forced83x61 resampling. Preserve the
 83x61 template role. CComponent uses SpellInt for its two smaller size classes,
  SPELLSCR for its two larger classes; do not invent a43x34 scroll export from this.
- `QuickSpellPanel` positions SPELLINT at(2,7+50*i), with an explicit48x36 disabled
  overlay. `StackInfoBasicPanel` positions effects at(15,206+38*i), with duration
  text ending at(+46,+36). The48x36 effect role therefore has concrete consumer
  geometry, including a text overlay that art must remain readable beneath.
- SPELLBON is also consumed at an explicit32x32 Rect in CHeroOverview (spell list),
  despite the58x64 source/schema role. Include a32px readability review, not an
  unrequested replacement source resource or universally native-size claim.
- **iconImmune binding:** CSpellHandler loads graphics.iconImmune as ImagePath;
  CBonusTypeHandler's SPELL_IMMUNITY branch with a valid SpellID returns that
  spell's getIconImmune(), before generic subtype/value icons. CStackWindow builds
  its BonusInfo image through bonusToGraphics, then uses CPicture directly—no
  resizing/clipping in the bonus-row constructor. The row has a52x52 frame at
  image-origin(-1,-1), description at(+60,0) in137x50 and source text at frame
  origin(+4,+38). Thus the ordinary card offers a50x50 icon interior; **50x50 is
  this consumer's layout target, not a measured universal immunity PNG size or
  cleared template**. No matching immunity template/live resource was established
  here. Do not substitute the48x36 effect frame or claim arbitrary images autoscale.
- Follow-up on other bonus-icon consumers: CStackExperienceDetailsWindow explicitly
  scales image-path row icons to32x32, centered in the row-name cell. WikiCreatureContent
  budgets ICON_SIZE51 and ICON_COL55, but places an unscaled CPicture at MARGIN+2,
  vertically using(rowH-51)/2; this is not a51px resize. Commander master-ability
  icons also wrap native CPicture dimensions without a fixed-size resize. Therefore
  the request manifest needs32px secondary-readability QA and native50px card/wiki
  fit checks, not a claim that every immunity consumer uses one enforced dimension.
  CAnimImage's Rect constructor confirms explicit scaledSize32x32 for the hero
  overview SPELLBON consumer; ordinary native-frame constructors do not do that.

References: client/windows/CSpellWindow.cpp (SpellArea), CCastleInterface.cpp
(scroll constructors), CHeroOverview.cpp; client/battle/QuickSpellPanel.cpp,
StackInfoBasicPanel.cpp; client/widgets/CComponent.cpp; client/windows/
CCreatureWindow.cpp (BonusesSection rows); lib/CBonusTypeHandler.cpp and
lib/spells/CSpell{,Handler}.cpp. Actual mounted font/edge/tooltip presentation and
selected-file rights still require their separate gates.

## Prior artwork checkpoint — isolated Logistics draft, no mount

`build/new-horizons-linux/research/logistics-icons-offer1/outputs.json`
(SHA716f6726132fe7fa76d4340012a2ce86084560104f8333810a5cc3f3b669d22b)
offers6 editable SVGs and6 RGBA PNGs for ForcedMarch/Quartermaster/Pathfinder,
32/64 each. Original transparent vector foregrounds; CC0 dedication/provenance
and source/output hashes included. No purchaser/template pixels or fonts.
Native-size offline preview inspected; dimension/alpha/rim and12 regenerated
SVG/PNG hash checks passed. Missing CairoSVG import and first resampling-rim RED
are preserved; bounded Pillow-only successor, no dependency installation.
These are provisional symbolic drafts, not final illustrations or GUI evidence.

Build confirmed future destination `runner/Mods/new-horizons/Images/`, NOT
Content/Images. Existing mastery-window lookup requests only `<iconKey>_64`;
32 remains a deliverable/future size. Content reports independent17-pin review
and byte-identical isolated regeneration at `testing/logistics-icons-independent1/`.
Build's `build/logistics-icons-packaging-review1.json` is inspected:17 pins,
6 PNGs/6 SVGs, exact package path/current64 lookup, conditional provenance only.
Eligible for a future isolated package proposal, not mounted or final-style approved.
No held profile, d90/root Images, gameplay source or active candidate was changed.
Mounted text fit, visual approval and ordinary two-family/save/dormancy journeys
remain open; native Logistics/Managed regressions do not satisfy them.

## Prior checkpoint — isolated receivers, not graphical acceptance

Delivered isolated session-runtime2, launcher-channel2, profile-lock1 and
inherited-profile-lock1 offers under `build/new-horizons-linux/research/`.
The inherited-lock independent summary is inspected:30 MOCK controls, exit0,
five original pins unchanged, actual FD/child/dlopen operations denied. Returned
child-local handle ownership is retained before borrow/checkpoint; actual shared
open-description lineage still refuses. Equal inode/receipt is not authority.
Content reports source39 paired receiver/provider MOCK integration; its late-pin
error RED and original source offers remain preserved. Bash2 is unpromoted.
Source37's targeted14 mock/temp-FS controls independently passed; source36's late
environment/deadline dispatch REDs now refuse. No native default69/GUI acceptance.
Writer2 metadata EXIT0 crossed its rendezvous deadline: explicitly aborted, holds
released, resulting fresh approval forbidden; no primitive invocation/retry.

Separate Logistics attempt2 `build/logistics-native20-attempt2/result.xml` and
summary are inspected: actual20 tests, zero failures/skips, including3 NK2 cases.
Content reports35716 fences/14 writes independently matched; Frontend has not
rehashed that inventory. Original attempt1's19P1F remains historical. This is not
installed-v2, GUI, mastery-art or frontend family acceptance.

Next full frontend gates remain ordinary book/assignment/fresh-process persistence,
managed acquisition/cast/save, same-book actual panel replacement, remaining
hero/category/navigation usability and original licensed art. These are not
satisfied by the harness offers. Sole Content owns graphical execution; actual
bootstrap/admission/ownership/death and fresh graphical approval are still missing.

## Prior default69 refusal correction (no primitive or GUI)

Inspected `testing/default069-legacy-book1/native-primitive-writer1-refusal-correction.json`
under `build/new-horizons-linux`: metadata writer exit1 occurred at its FIRST
census/gates before receipt publication, not the second. The earlier incorrect
trace label remains preserved. Receipt/completion/temporary/attempt artifacts
were absent and approval remained ad6c; no primitive invocation or retry followed.
This is neither a process-absence proof nor a permanent blocker for the full goal.
Runtime binding25's nested Mods replacement RED is separately preserved; Content
reports a successor final FD/path check with controls pending. No approval inferred.

## Prior default69 checkpoint — attribution source and primitive refusal

Isolated attribution source2 is delivered and independently mock-reviewed:
`research/default69-attribution-source2/` under `build/new-horizons-linux`.
Positive-only reader returns UNKNOWN, never death from an empty census. Failed
close revokes numeric capability before the call; no retry authority survives.
Source1 consumed-close/reused-FD RED remains preserved. Native reader/producer
acceptance is still separate from those16 mocks.

Runtime creator source24 received a scoped four-control temporary-FS review;
whole83 input prehash refused on a missing working-path historical RED artifact,
so no full83 seal was claimed. Session/launcher retained-identity/death/ownership
binding remains unadmitted. See `research/spell-roster-ui/default69-creator24-review.md`.

Inspected `testing/default069-legacy-book1/native-primitive-freshness-refusal1.json`:
actual approved-command invocation exit1 at initial freshness guard, before
attempt/result/terminal publication or child acquisition. Input/interpreter hashes
matched the offered approval; later inspection age215.281s is NOT execution timing.
No retry, process census, kernel-primitive PASS or GUI GO follows. Fresh separate
approval is required for any later attempt; ordinary default69 graphical and full
frontend acceptance gates remain outstanding.

## Prior default69 lifecycle checkpoint — still no graphical admission

Delegated isolated controller source3 is in
`build/new-horizons-linux/research/default69-lifecycle-source3/`:
controller f767667c, tests739dc59a, contract95e1babb. Actual23 mock controls passed
locally; Tester independently reports original23 plus residual-live-group and
all3 postcreation-handover controls. Source1/2 and their actual REDs remain intact.
Attempted-role uncertainty blocks destructive runtime/X release; forced client or
live/uncertain group cleanup cannot become ordinary exit0. Exact normal_exit and
forced_cleanup fields supplement raw_launcher_exit. Role identity publication is
explicit; missing identity is not clean. Native adapters must honor returned
published/error/normal flags even after partial exit-file publication.

Tester copied the controller into lifecycle_controller.py for adapter preparation
ONLY. No adapter execution, registration/outer-crash recovery, full lifecycle,
READY/GO or GUI acceptance follows. Final conjoined teardown/notification and
GUI outcome remain distinct: proven clean teardown can release holds on a GUI RED,
but unsafe/uncertain cleanup must retain holds. Next: exact adapter/attribution
review and Content's assembled finalizer/batch route; full frontend gates below
remain incomplete.

## Prior source-only checkpoint — bounded tooling is not frontend acceptance

Private owned-process ledger source3 retains source1/2 and their uncertainty REDs.
Actual-helper mock20 passed locally and independently (Tester reported0.026s);
registered-handle/discovery/final-inspection uncertainty stays sticky across retries.
No real pidfd adapter, pre-spawn containment, integrated runner or native execution
is accepted. Reports and offers are under `build/new-horizons-linux/`:
`native-compile-owned-process-source3/` and
`research/quick-spell-roster/containment-proposal2-feasibility-review.md`.

Static-clean-entry source2 independently passed six in-memory controls0.001s;
manual instruction/layout review applies to the unchanged42-byte entry. Neither
an ELF file nor a native process was produced by that review. See
`research/quick-spell-roster/static-clean-entry-source2-review.md`.
Service/user-namespace feasibility, atomic unit retention, first dynamic loader/
preload/import closure and original activation deadlines remain separate gates.

Tester reports default69 geometry/matcher25 offline controls passed, but the
full route/lifecycle is not admitted. Menu source-frame alias RED and original
Arrow full-opaque mismatch remain preserved; private native-resource decoding
and border-safe historical matching are not mounted-lookup or live GUI proof.
Next frontend verification remains ordinary book/assignment/fresh-process
persistence and managed acquisition/cast/save, followed by actual same-book panel
replacement, remaining hero/category/navigation usability and original licensed
art gates. Optional tooling work does not discharge any of these requirements.
No change to frozen publication or sole-Content graphical ownership.

## Prior checkpoint — default051 readback2 and separate widget prototype

Content's READBACK2 actual teardown is now inspected: client exit0/97.570s,
session97.722s, exact18-input read-only route,192 clean samples,5418 unchanged
fences, no save progression or post-confirmation input/capture. Frontend offline
comparison of all8 actual click/key screenshots found exact header/stats and
body equality against the separately reviewed four readback1 click bodies:
`testing/commands-static/default051-readback2-frontend-independent/screens.json`
under `build/new-horizons-linux`. Eight screenshots are not whole-screen,
overflow, book, QuickPanel, managed070 or Windows acceptance. Readback1 exit130
and expired coordination GO REDs remain immutable; publication is separate.

Positive-widget source3 compiled/linked, followed by separate LOCAL-symbol
inspection tail; original uppercase-T inspector RED retained. Runtime split
cleanup repair stops reader outside interfaceMutex, then releases GUI holders
under the existing lock AFTER endNetwork. Later native-cancellation tagged
no-engine driver/test source is a DIFFERENT offer: actual FIFO/weak closure,
queue receipt and lifetime observer, no Engine construction. Seven-source static
controls passed; native cases/mutants, host-access guardian and execution remain
pending. No registry-negative, SDL/widget or populated-holder proof inferred.

Final47 was reported committed/pushed as `d90c2ea7ae80456eae06f17f7286cf8debd8e705`
(tree459472, parentdb2f); this does not establish new GUI/default70/release acceptance.
Normal-player-content exporter subsequently passed its separately scoped native
case; candidate949/ordinary acquisition still require Content's own admission.
Older950/public413 and previous exporter/GUI REDs are not relabeled.

Four NEW unregistered `client/tests/` files implement a positive-only test-driver
prototype: `QuickSpellWidgetDriver.h/.cpp`, `QuickSpellWidgetProbe.h`, and
`check-quick-spell-widget-overlay.py`. No tracked EntryPoint/QuickPanel/CMake/ABI
edits or prototype rendering were made. Registry negatives remain DISABLED:
GUI dispatch already holds nonrecursive interfaceMutex, but unlocked/detached AI
paths prevent inferring registry-transition safety from that lock alone.

Inspected `build/new-horizons-linux/widget-prototype-controls2-i-fixed/summary.json`:
pinned6 sources, root unchanged, exit0/0.103215s, checker b025f4d2. STATIC controls
only; expected entry4dc759d3/quickff627517 are not offered/built overlays. Original
controls1 missing-seam RED and independent mutable-source/no-prehash RED remain
separate. Previous52fc/2dac checkers are preserved under
`research/quick-spell-roster/widget-prototype-original/` in that build directory.

Next: reviewed private overlays, explicit EntryPoint-object REPLACEMENT and proof
of old QuickPanel archive-member exclusion; actual native reader/cancellation and
widget gates remain unproved. Content alone may render after fresh GO and must
revoke lease.token BEFORE quit confirmation, testing queued post-latch rejection.
Preserve100/180/200/250/300 limits and normal teardown. This harness is NOT a
substitute for ordinary acquisition/cast, canonical preference fresh-process
reload, broader hero/category/navigation usability, final art or full-goal gates.

## Latest future source — quick-slot roster guard (UNCOMPILED)

Build leased QuickSpellPanel.cpp/.h + new unregistered tests; implemented3-file
source offer at `research/quick-spell-roster/source-ready.json`. Actual battle
admission precedes configured spell metadata/icons and autofill lookups; decoded
excluded preferences stay reserved blank/noncastable/no marker/no autofill and are
not erased. Truly empty slots keep eligible autofill. Existing BattleWindow caller
unchanged: getSpells supplies freshly sanitized keyboard IDs.

Click/popup/selection closures retain weak original CPlayerBattleCallback identity
and heroID, never panel/hero pointers. Resolve CURRENT battle and hero each time;
same-context panel recreation survives, changed/expired/missing context rejects
before cast/storage. Missing callback registry throws in existing getBattle; narrow
lookup helper returns absence and checks actual battle state before hero access.
create now clears old configured-marker widgets with other children.

New `client/tests/check-quick-spell-roster-routing.py`:2 STATIC tests and10 in-memory
source mutants passed. Initial harness2ValueErrors retained (missing token prior to
index); repaired explicit presence assertions. Not native logic/widget execution.
CPP UNCOMPILED, offered Content independent review. Subsequent null player/callback
lookup guard source repair preserved first offer. Build then identified unscoped
preference writes: changed explicit valid selection to CSpell::getJsonKey AFTER
context/roster checks; unchanged decode reads preserve legacy bare core IDs, excluded
preferences never rewritten. Latest `source-ready-canonical-key-fixed.json`, prior
CPP/tests hash-preserved, header unchanged;2 static tests/12 source mutants passed.
Actual managed-profile persistence/reload untested. Source-only reviews do not prove
native context behavior. Actual context replacement,
old saved/new installed preference, invalid IDs, storage preservation, rendering,
keys/popup and native/full-link gates pending. No BattleWindow/CMake/product-rules
edits, imports or GUI run by Frontend.

Later inspected actual integration2: QuickSpellPanel11/18 and corrected
CSpellWindow12/18 objects compiled; first build RED retained from Runtime fixture
MetaString::toString missing translator argument. Repaired
`magic-consumer-integration2-translator-fixed/summary.json` configure/build/native0,
234=223PASS/11SKIP/0FAIL, client2/4 and test4/4 links. Fences true, root client4a4f6cbb/
facade3070c532/test5fec2b09. Corrected frontend source now compiled/linked, NOT actual
managed-profile preference reload/context-widget/QuickSpellPanel GUI acceptance.
Managed opt-in profile and independent next gate remain separate.

## Future source — spellbook saved-roster admission (now compiled/linked, not GUI)

Build separately leased ONLY CSpellWindow.cpp/.h after the actual Runtime public
NewHorizonsSpellAvailability.h appeared. Implemented copied rosterSpellIDs cache
through const world/battle free-function APIs; reject missing actual battle rather
than world fallback, skip null definitions, admit BEFORE school/level lookup.
Legacy-school counting checks same cache before canCast/.at; processSpells checks it
before normal castability OR selection/show-all. Show-all bypasses possession only,
not saved roster. No client-derived rules/defaults or cast-validation replacement.
Actual selection/show-all route is QuickSpellPanel.cpp138, not ordinary book alone.

Offer `research/spell-roster-ui/source-ready.json`:7 static source-order assertions
and whitespace checks only, UNCOMPILED/unrendered; all held37 hashes unchanged.
Offered Content context/cache review and Runtime API-seal confirmation. Subsequently
read `commands-static/spell-roster-ui-source-independent.json`: bounded SOURCE
approval, exact CPPbf63bc7e/header73ed497d/API1e1ad2e2. Later prebuild SOURCE defect:
BattleInterface getter throws on missing registry, and a CBC may contain null state.
Build authorized narrow repair, preserved originalbf63 CPP; new
`source-ready-missing-battle-fixed.json` catches runtime_error ONLY around getter,
checks player/callback and actual CBC state BEFORE active-school metadata, returns
cleared caches without world fallback. Three static source mutants rejected, not
native exception/widget execution; header unchanged, repair uncompiled/re-review. Constructor-only book-local
cache; no context-replacement refresh/invalidation acceptance. Future actual
API/native/object/link plus old NULL/v1 imported-Missile exclusion, valid/invalid v2,
battle/world conflict and legacy tab/search/pagination GUI gates remain. No import,
activation, CMake, new art or frozen candidate edits by Frontend.

Subsequent actual registered full integration inspected:
`magic-full-integration1` first build1 retained (Runtime consumer fixture const
callback conversion errors59/60); actual CSpellWindow object363/516 compiled.
`magic-full-integration1-callback-fixed/summary.json` configure/build/native0,
204 total=195PASS/9SKIP/0FAIL, client51/53 and test53/53 linked. Input/copied CPP/
protected fences true; clientd0f71a77/facade5ccca3ab/testf5627b19. This advances UI2
from uncompiled offer to compiled/linked, NOT imported-Missile/new UI pixels,
QuickSpellPanel/show-all or default activation acceptance. Old950 remains separate.

## Current future-source checkpoint — saved-detail navigation implemented, NOT413930

User AFK explicitly authorized continued implementation without waiting for definitive
art. Build sealed independent read-only release-413930-source (no hardlinks), then
explicitly leased only future HeroGrowthWindow.cpp/.h plus new navigation helper/test.
Implemented FOUR read-only detail tabs using existing80x32 button resources at y332:
Growth, Leadership, Siege, Masteries; keys1..4. Actual independent saved optional
views determine availability. Existing totals/formulas/saved mastery formatter are
unchanged, no query replies or points spent. Selected available section persists
through same-hero refresh; missing selection falls back to first available family.
Refresh rebuild resets scroll (NOT scroll-retention claim). Switching sections resets
both text and scrollbar to top; existing656x108 body/700x560 window bounds retained.
This addresses real saved-mastery readback scroll friction, not the entire hero redesign.

Files: `client/windows/HeroGrowthWindow.cpp/.h`, NEW
`client/windows/HeroDevelopmentNavigation.h`,
`client/tests/HeroDevelopmentNavigationTest.cpp`. First source offer retained at
`research/hero-navigation/source-ready.json`. Content found a SOURCE RED: actual
CSlider::setValue ignores its argument; using it left thumb/value stale despite
resetting text. Preserved original CPP as HeroGrowthWindow-slider-red.cpp; changed
ONLY owned callsite to public scrollTo(0), NOT shared Slider.cpp or frozen source.
Added explicit multiple-available FIRST fallback tests (removed Masteries -> Leadership/
Siege, and absent -> multiple), beyond16 defensive masks. These are NOT sixteen
reachable game contexts or widget/slider/GUI coverage. Latest repaired4 hashes at
`research/hero-navigation/source-ready-scroll-fixed.json`; current4 held for Content
source review and Build registration/compiler authorization. Subsequent independent
`commands-static/hero-navigation-source-independent.json` PASS inspected, including
cleanup/geometry/optional/math boundaries and retained slider-call RED. Build then
compiled actual standalone helper C++20/-Wall/-Wextra/-Werror0 and ran test0; read
`research/hero-navigation/native-test.log` PASS. This covers pure state only, not
widget/slider/native font/covered-key/GUI behavior. Build's separate180s OBJECT-ONLY
HeroGrowthWindow OBJECT-ONLY compile subsequently passed0; read actual
`research/hero-navigation/native-scope.json` binding all4 current hashes and helper/
object scopes. Source4 held unchanged. No full target registration/link/GUI or release
acceptance. Suggested a future Build-owned private translation stress fixture to
make Siege+Masteries both overflow, then short Growth/Leadership removes slider and
switch-back recreates it; diagnostic text must not be reported as normal user-data
polish. No such fixture or candidate edited/created by Frontend. No CMake/config/live-art/commit by Frontend.

Runtime future category APIs remain uncompiled/native-pending, but Build later
explicitly leased category UI SOURCE in ONLY CCreatureWindow.cpp/.h. Implemented
copied optional CreatureCategoryView BEFORE preview fakeNode creation: a CStack uses
its OWN const BattleInfo's inherited battleGetCreatureCategory callback; else real
CStackInstance uses its actual public GameCallbackHolder.cb->getCreatureCategory.
Inspected headers: CStackInstance.getCallback override is private, so that draft
access assumption was corrected before READY, with no lib/API access changes.
No global GAME/current-world lookup or alternate fallback; even null/absent battle
context cannot fall into the world's branch. Bare/no-context/unmapped cards remain
unlabelled. A new plain28px CategorySection exists ONLY for an actual view, after
MainSection and before spells/bonuses; names/descriptions use saved text IDs, help
includes sourceRulesetId/rulesetVersion. Existing textured background, no new art;
stats/bonuses/recruitment/upgrades/capacity/math unchanged. Runtime confirmed the
positive out-of-range/null entity guard exists but native tests remain pending.

Initial Category UI2 offer at `research/creature-category-ui/source-ready.json`
retained with exact CPP/H copies: Content found a SOURCE lifecycle RED, existing
commander update rebuilt sections without recapturing category/resetting its widget.
Repaired with private shared resolveCategory called initial/pre-fake-node and after
commander target update/before rebuild; categorySection reset beside other sections.
Latest `source-ready-lifecycle-fixed.json` remains UNCOMPILED/unrendered, offered
Content re-review and Runtime callback ACK. Commander mapped-to-unmapped/changed
context rebuild still needs actual verification; canonical14 roster reachability
not inferred.28px geometry needs actual minimum-resolution/long-text testing, not
an automatic-fit claim. Subsequently read Content's
`commands-static/category-ui2-fixed-independent.json`: bounded repaired SOURCE
approval, exact CPP3bb66e86/headerf5ed8631, retained first2 verified. This is only
approval for future combined freeze; no object/link/GUI/roster acceptance. NAV4
hashes independently checked unchanged.

Subsequent Build-owned future36 initial combined build FAILED1:
`category-navigation-build.exit/.log`, Ninja stopped after396/442. Inspected actual
StateTest.cpp127/173 nonexistent CreatureID::PIKEMAN plus incomplete
CObstacleInstance/CampaignState serializer instantiation errors. Verified all36
current and frozen copies against category-navigation-integration36/identity.json
with zero mismatches. Routed exact test-source failure to Runtime/Build; no Frontend
or production repair, no Native25/registered-NAV run or link/GUI acceptance from
this failed build. Initial RED retained. After reviewed Runtime fixture2 repairs,
read category-navigation-fixed-build.exit0 and actual final client46/48/test48/48
links. All36 live and category-navigation-integration36-fixed copies hash-exact.
This establishes the repaired combined build only; initial Native25/registered NAV
execution and actual future GUI remain subsequent gates.

Read revised `testing/future36-ui-plan/PLAN.md`: separate proposed ordinary world
four-army cards, old5374 navigation/readback, and reachable land battle sessions;
no fixture/export/candidate/GO inferred. Ordinary matching world/installed metadata
cannot prove saved-context discrimination; old unmapped Pikeman cannot prove legacy
mapped-Pixie absence. Commander refresh currently has no ordinary caller (level-up
creates a new window), so changed-context refresh needs explicitly scoped actual
widget coverage. Growth has at most four extra rows; two overflowing panes and all16
availability subsets are not assumed reachable. Distinct translated saved names/
descriptions and provenance are required in later synthetic context fixtures.
Controlled Build world/battle negative leases remain separate from GUI permission;
frontend6 stays held through restoration and clean binary verification.

Later owned6 final staged review completed: full507-line diff inspected and all6
index/current/readonly copies/offer/prior fixed approvals identical; report
`research/creature-category-ui/foundation-owned6-review.json`. Build reported exact37
foundation commit0afc38f09f5e391dcfdb4f6af1f3fa0eea77e987 separately; no default0.6/
release/GUI inference or private950 relabeling.

First private0.6 WORLD4 GUI did NOT reach gameplay. Read actual
`testing/category060-world-gui/summary.json` and teardown.json: scenario description
at70.160s, BEGIN rejected before dispatch by setup reserve at elapsed>=98 (no exact
rejected timestamp recorded). No cards/new game/save. Normal exit179.407s/session
teardown179.874s,354 clean samples,950/source37/map/purchasedData/native fences exact,
empty save inventory. Preserve this SETUP_TIMING_RED; next is a separately prepared
faster known setup route and fresh pause/GO, not weakened guards or reused permission.

Distinct FASTSETUP WORLD4 subsequently reached actual ordinary cards. Read
`category060-world-gui-fastsetup/teardown.json` and personally viewed screens
0080.366/0100.037/0119.934/0148.964/0169.628:20Pixies Core,20Air Elementals Elite,
2Phoenixes Champion,100Pikemen no category row; Core left-help resolves description
and new-horizons:creatureCategories(version1). Elite/Champion help not opened.
No saved/current-context discrimination, restart, battle or navigation acceptance.
Normal exit227.826/session228.019,449 clean samples, all structural fences true,
empty saves. Target200 MISSED; mandatory250/hard300 met. Actual shown viewport only,
not minimum-size/long-text acceptance; blank trait icons remain visible broader gaps.

First NAV5374 journey retained UI-invariant guard RED after Growth click: tab2/key1
rejected BEFORE dispatch, no bypass. Read actual teardown and viewed0135.048 screen
in `testing/category060-navigation5374`: four tab labels visible, Growth selected,
21/28/7/14,last3/4/1/2,mana10/14,MP1087/2028. No Precision/complete tab/key/overflow
acceptance. Normal exit190.010/session190.031,374 clean samples, all fences true,
only unchanged5374 input save. Tester owns offline ROI diagnosis and separate retry
proposal; no product defect inferred or frontend source repair made.

Distinct strict-interior NAV retry: read teardown and actually viewed all8 click/key
screens153.395..158.566 in `category060-navigation5374-interior`. Bodies match Growth
(no extras), Leadership100/900/100%, Siege Expert/x4/three100% controls plus limitations,
and Precision ACTIVE distance/wall-only restriction text. All fit shown viewport;
no overflow tested. Keyboard1..3 preserve white Masteries mouse-hover border while
gold selected border moves; not a single-border/covered-key claim. Tester later
confirmed bounded content PASS after viewing all8 full screens; read actual
click-key-content-independent.json: four distinct bodies, each click/key pair exact.
Normal1280x800/110% text fit only; no overflow/minimum-viewport acceptance. Exit207.617/session207.743,409 clean samples,
fences true/only unchanged5374; target200 MISS retained,250/300 met.

First BATTLE4 read actual summary/teardown at `testing/category060-battle4`:
ordinary pursuit reached20Pixies/20Air/2Phoenixes/100Pikes versus4+4Pikes, but NO
cards executed. Actual gear229,750 differed from prepared ROI/allowed rectangle;
false binding refused, no waiver/rebind. Actual Options/QuitDesktop/mouse confirmation
observed. Exit170.800/session171.213,337 clean samples/all fences exact/no saves,
all limits met. This is preparation-layout RED, not demonstrated product defect;
no category-battle card/effect/AI acceptance. Separate corrected preparation needed.

Distinct BATTLE4_LAYOUT safety release retained forced-exit RED124. Read actual
`category060-battle4-actual-layout/teardown.json`: client284.308/session284.730,
561 clean samples/all input fences exact/no saves/PIDs/X absent; normal exit and
session-success checks FALSE, though raw elapsed is below300. No normal200/250 PASS.
Personally viewed four actual106.217..109.814 card screenshots: Core20Pixies,
Elite20Air,Champion2Phoenixes,100Pikes no category. Await Tester content verdict;
visible labels do NOT turn forced termination into clean journey acceptance.
Tester subsequently independently confirmed all4 images/Options; events stop at
gear110.570, right-ups complete by110.272, no quit-item/confirmation dispatched.
No timestamps establish the later gap's cause: not a proven product hang or image
I/O problem. Watchdog reserves20s from hard300, not normal250. No product repair
or retry authorized from this evidence. Old950 only, not new root spell-roster UI2
or imported-Missile acceptance. Future schema/canonical mappings/native
and actual old/unmapped/bare/conflicting-world-battle/min-size/tooltip GUI gates
remain required; source implementation is not runtime acceptance or413/947 scope.

External image-capable art workflow replaces further procedural art batches; no
user-approved motif/style or legal clearance inferred. Actually viewed external
master01 native-review.png: ring/core survives44/32, fine engraving/blue arc weak32.
Only technical feedback sent Artist; no live import or proprietary references in
product. Navigation requires no new art and remains independent of that feedback.

Read actual sealed Linux413930 build.exit0 and698/698 final client link. This is
NOT install/ELF/privacy/package/GUI acceptance; future tree changes were not inputs.
Await Build's scoped next compiler/registration and independent source review; remote
Windows full/cloud and release audit remain separate gates. Protected947/saves unchanged.
Later actual packaged Linux readback PASS inspected in
`testing/linux-413930-readback/summary.json` and actual02-precision-active.png:
source413930, packaging83cf5443e8ce11b87288297722bb32a3b3023633,1161-file manifest
e79a1b741060dda94dc571c26a370dd4603b6e8dbcaa895f5465faf83dbb8e5a; fresh5374 saved
Precision ACTIVE/L3XP2000/eightExpert/100Pikes+Ballista,21/28/7/14,last3/4/1/2,
mana10/14,MP1087/2028. Actual old scroll-based released UI, NOT future tabs.
Quit102.331..102.508/confirm102.891..103.069/normalexit103.097,203 clean samples,
full package/control/source fences intact/no new saves. No battle/effects/AI/F8QS/
future UI/native Windows/full-redesign inference. Windows FULL cloud build succeeded
separately; its exact artifact/package audit and publication remain Build-owned gates.

## Historical checkpoint — mastery26 boundary reviewed, convenience42 SOURCE_READY

Read actual `testing/mastery-gui-first/summary.json` and `mastery-reload-first/summary.json`.
Ordinary existing-Expert level2 -> Basic Sorcery secondary -> three mandatory mastery
cards; Enter/Esc before selection did not choose; explicit1 Volley + confirm accepted
and ordinary distinct save e5efe637bca25bd4bb765dc0c363e15b3bcb87d82e2837f84cb0cad25b51c2dd
was produced. Fresh process restored Expert Artillery3/active Volley+1 text, restrictions,
base18/24/6/12 and capacity100/825. Fresh reload normal quit183.120s passed. Initial
1x1 black-window setup, uncertain Gold/resource selection, and late490.3>450 first
quit are retained RED/caveats; no hang inferred. No actual combat/effect/AI/covered
popup/newly-Expert claim. Next boundary GUI was deferred for Runtime AI valuation
characterization; no Frontend compiler or GUI authority is implied.

Reviewed exact82 `mastery-integration-review/identity.json` AND copied files: owned
12UI/test +14art/source match current hashes and previous12-file source-ready set.
Approved ONLY that owned26 unactivated foundation boundary; report
`research/mastery-ui/foundation26-review.json`. Default0.4 mod, convenience and
Artist Sorcery drafts excluded. No activation/publication/full-goal acceptance;
no edits to held82/925/891. Build alone integrates and chooses commit timing.
Later exact86 `mastery-integration-review-ai86` offer: independently hashed current
owned26 AND immutable copied files against prior82; all26 unchanged. Explicitly
approved only that owned unactivated foundation boundary, report
`research/mastery-ui/foundation26-ai86-review.json`. Default0.4, convenience and
Artist drafts remain excluded. Build reports broad40/40,140(138+2),61x2(58+3),
128(126+2),39(38+1) green and strict BE two-negative then restored clean-six; this
owner hash review does not independently certify Runtime code or GUI AI effects.

Separate convenience implementation now has an exact42-file source/art offer at
`research/convenience-art/source-ready.json`: ONE existing CPP
`client/adventureMap/AdventureMapWidget.cpp`, NEW independent generator/auditor/note,
and38 new outputs. After teardown,18SVG/18PNG/2JSON generated and independently-root
reproduced exactly;421 old outputs byte-identical (459 total). Separate auditor
rejects six negatives (blank/wrong size/opaque/visible trait edge/swapped frame roles/
embedded SVG image); native contact inspected, not claimed finished painterly art.
Evidence `research/convenience-art/{audit,negative-audit,before}.json` and contact-native.png.
Initial getdata deprecation warning retained; current auditor uses portable pixel access.

Build found raw items-array hook would assert when build() reads object dimensions.
That source-review RED is retained; repaired hook wraps ONLY items in a sanitized
JsonNode OBJECT, appends after base build, requires mounted optional resource and
excludes portrait layout. No base replacement, default activation gate or save/rule
changes. Build-authored fragment is `Mods/new-horizons/Content/config/widgets/nhConvenience.json`;
bonus file `config/newHorizonsConvenienceBonuses.json` remains Build-owned, with
objects `{graphics:{icon:...}}` preserving all original descriptor fields. Exact
help keys end in `.help`; existing shortcut/blocking callbacks remain the only actions.

Content independent convenience42 source/art review now PASSED (read actual
`testing/convenience-art-independent/source-config-independent.json` and reproduction
report):42 hashes match,38 reproduced exactly, old421 unchanged, six negative
controls rejected, native contact actually inspected, four Build data tests passed.
Sanitized-object/base-first/optional-resource source path reviewed against build().
This is source/assets-only, not compiled/native-merged/UI/Windows/final polish.
Bare-array RED remains recorded; held42 unchanged. Build has a separate private-only
0.5.1 composer; current0.4 and frozen925 remain unchanged.
Subsequent Build native diagnostic found a REAL private-composer mounting RED:
module filesystem exposed SPRITES only, so a listed bonus file was inaccessible.
Build reports repaired private composer with inline ten graphics patches and explicit
Content mounting (outside82); native ten icon paths resolve via actual SPRITES
fallback, creatureNature/description propagation/descriptions match and SPELL_IMMUNITY
control is unchanged. Prior mounting/probe build REDs retained. This is a bounded
Build-reported native result, not yet our inspection of its exact report and not
compiled hook/GUI/hidden-value-subtype coverage by inference. Frontend42 unchanged.

Subsequent semantic/visibility RED confirmed from BonusEnum and actual native JSON:
NO_RETALIATION is inability of a paralyzed unit to retaliate, NOT the common
Naga/Vampire BLOCKS_RETALIATION trait. Asked Build to replace that mapping with
BLOCKS_RETALIATION using existing noRetaliation art; no new rule or drawing required.
Build authorized ONLY the provenance-note correction and minimal original Siege
Weapon text as a data-owned presentation exception. Corrected42 offer is now
`research/convenience-art/source-ready-retaliation-fixed.json`; verified ONLY
CONVENIENCE_ART.md changed (SHA f0c2bd4308857af347c911363c9bdbc496ade5ae7087bdf0f8ad31f47227067d).
CPP/art/both generators unchanged; previous source-ready.json and resolver evidence
remain preserved semantic-RED history, not silently relabelled. Authorized text:
`{Siege Weapon}\nThis unit has the siege-weapon trait.` Native expectations must allow
only this explicit description change, not claim blanket description identity. SIEGE_WEAPON also has empty default text;
CCreatureWindow.cpp1096 omits blank/hidden entries. Do not weaken that filter or claim
ten visible traits from ten resolved icons. Actual Naga/Vampire and Undead UI tests,
plus preserved paralysis/spell/blank-siege behavior, are requested from Content.

Later bounded progress: inspected actual `convenience-hook-object-build.log/.exit`:
version task + ONLY AdventureMapWidget.cpp object, exit0, no client/facade link.
Read and compared existing `convenience-corrected-{mastery-native-first,convenience-native-corrected}.json`:
ten nonempty description/resolved-icon pairs, creatureNature/propagation stable,
ONLY authored Siege description differs, NO_RETALIATION and Magic Arrow immunity
control identical, optional fragment absent baseline/present mounted preview.
This confirms the stated loader/object scope, NOT ten rendered traits or runtime
controls; source42 remains held. No tests or compiler self-launched in this review.

Mastery exact86 was committed/pushed by Build as dd6f6e07af7e445cec863082efebb34cce5dab77;
locally verified86 paths, author+committer thegandalf196, and clean owned mastery
windows. This is foundation only, not activation/release/full GUI acceptance.
Reviewed actual read-only `convenience-integration-review46` base dd6: all corrected
owned42 copied/current/offer hashes match; explicit boundary approval recorded in
`research/convenience-art/owned42-review46.json`. No held42 edits. Build's four data
paths and Runtime's new test-only creature fixture remain separately owned.
Read `convenience-priority-full-preview.json`: private sentinels exercise value/
subtype resolution, real stack custom override and spell-special EMPTY result even
with competing descriptor paths; custom remains above spell-special. Not a ten-default
icon report or GUI proof. Build reports probe compile10/two context runs0, preserving
prior setup API/include/enum REDs7/8/9; independent full gate review still separate.

Subsequent COMBINED link build inspected: `combined-dd6-convenience46-build.exit`0;
log links vcmitest, libvcmi.so, libvcmiclientcommon.a and vcmiclient. Verified all133
current hashes against its held manifest (including default mod0.4). This is dd6+46,
NOT86-only, and NOT a frozen candidate/GUI/release claim. No source drift found.

Private947 now sealed at `combined-dd6-convenience-private-first`: read BUILD-IDENTITY
(dd6+46, module0.5.1, not distributable); verified SHA256SUMS digest
64ac2d34817e97e12c33a434c90105516becbba90d2266c1c6f663437f0a1ee9 and all20 new runtime
PNG/animation file hashes against corrected offer. This is NOT a full947/ELF audit.
New fixture build0/baseline0 with actual XML one expected opt-in skip; activated
run exit1 before cases: `Failed to find mod vcmi-test`. Read actual log, checked all
held134 hashes unchanged, notified Build to repair private fixture-root setup only.
No41-pass/map-export claim from that RED;947 unchanged. Old925/e5 remain protected.
Third private runner later passed: read actual convenience-fixture-assets-activated.xml
(all41 cases, no skips/failures) and exit0; independently verified held134 unchanged.
Second setup RED (missing DATA/LCDESC after fixing test-root location) also retained;
Build repaired only private runner's authorized read-only external Data symlink.
Read export manifest: NHConvenienceArmy hash40405710905aedf86ac54e6d1e0142e9e5db2013a90b1ae9c177b3550f7a51b5;
ExpertChoices2f7d02ea/NewlyExperte5b02f04 unchanged. Fixture source is ordinary L1/XP0
100Pikemen/20Vampires/20VampireLords/20Nagas + Ballista, no XP/scripted gameplay.
Suggested separate bounded QS/QL and trait journeys to Content after independent947+
map audit/Build grant; basic Vampire must not be labelled life-draining like its Lord.

First actual947 GUI now revealed a presentation RED. Viewed actual
`testing/convenience947-gui-first/03-quick-save-tooltip-red.png`: buttons fit below
minimap, QS produced real Quicksave671560 bytes/SHA
dee34173c79fee9e00d5d8bdca13a9530506e36dce2c8e34a4f20a2a291b678a, but hover displays
raw `vcmi.adventureMap.quickSave.help.hover`. Read readHintText292-309: STRING is a
PREFIX to which .hover/.help are appended, not a leaf key. Both configured prefixes
and our note need correction; prior source review missed this. Build owns two-string
fix/regression/new freeze, NEVER edit947. Requested note-only42 correction/reseal;
Authorized note-only correction completed: `source-ready-help-prefix-fixed.json`,
note SHA11d16e6b25a1434df6e7e2eb901d266ce58519953c7892654ad1af5d8d91d79c,41others unchanged.
Reviewed NEW read-only `convenience-help-prefix-review46`: copied/current/latest42
match; compared old46 exactly fragment(two strings),test,note changed,43others same.
Explicit source-boundary approval at `research/convenience-art/owned42-help-review46.json`.
New candidate `combined-dd6-convenience-help-fixed` is distinct from old947; Build
reports same binaries/module, native prefixes/old-raw negative lookup0 and four data
tests0. Still awaiting independent new candidate gate and actual GUI. Explicit
PAUSED/ready ACK sent for its pending lease; NOTGO, no heavy work until teardown/cancel.
CPP/art/generators unchanged. QL initially grey; no move/QL/cards/F8F9/battle/end-turn
proof from this stopped run. Build verified normal quit242.18/exit265.55 and complete
teardown/protected inputs; shutdown XIO retained, no hang inferred.

Help-fixed947 actual GUI bounded PASS: read `testing/convenience947-help-fixed-gui/summary.json`
and actually viewed Lord card09. English QS/QL hover+rightclick help, initial disabled
QL, button QS -> safe WEST move -> button QL/confirmation restores position/L1XP0/
army100+20+20+20. MP1560/1560 observed AFTER restoration only, no numeric movement-delta
claim. Quicksave671307 bytes/SHAecb86e25fad4311784fd1675724902f8b8892022fc9cd11cac17d7f49033d3b3.
Four actual cards: both Vampire types Flying/No Retaliation/Undead, only Lord Life Drain
text100%, Naga no-retaliation not Undead, Pike Jousting Immunity not Undead. Blank Life
Drain/Jousting icon cells remain a broader gap; sent future-only specific script subtype/
CHARGE_IMMUNITY mapping proposal to Build, no new edits or generic all-script icon.
No F8/F9/fresh-process/battle/endturn/mastery proof. Quit349.24/confirm358.4/exit358.577,
707 clean samples, complete teardown/protected inputs; helper ValueError/shutdown XIO
retained. Source48 committed/pushed by Build as a3d6a7271d947e75a9856f7c9998b0fbd3b53781;
verified48paths +author/committer identity. Default0.4 unchanged; existing candidate
remains dd6+declared deltas, NOT relabelled/rebuilt from new commit. Explicit PAUSED
ACK for next same947 NewlyExpert stage1 (no-mastery+namedL2 save).
StageA later completed: read actual `testing/mastery-newly-expert-help947-first/summary.json`.
L1 Advanced Artillery+7Expert -> ordinary1000XP Seer -> L2 gains3/4/1/2 -> Expert;
actual scrolled readback no mastery chosen/future Artillery eligibility/no awaiting
text. Base=total18/24/6/12, mana10/12, MP1628/2028, cap100/825, Ballista base x4.
Named NEWGAME-ne2 save676018 bytes/SHAaaea7743b9c8b826111549616301fc50c67ec33027d5baa65c6de581cf7195bc.
This is UI absence readback, not independent serialized pending-field inspection;
L2 XP not separately captured. StageB omitted past210 cutoff. Own300 quit target
MISSED: normal quit387.6/exit388.789 before400,767 clean samples and complete verified
teardown; protected controls intact. Fresh L2 reload -> L3/choice/save needs separate
proposal on SAME947, not activation/other-family creep.
Subsequent fresh run inspected at `testing/mastery-newly-expert-help947-reload/summary.json`:
L2XP1000/eightExpert/no-chosen/future-eligible readback and second ordinary1000XP ->
L3 gains3/4/1/2 +three unselected mandatory cards are evidenced. TIMING/COMPLETE
JOURNEY RED:300 guard blocked planned Precision call315.5; cleanup372.873 resolved
Precision solely to exit, normal exit374.585 AFTER mandatory350. No individual Quit/
confirmation timestamps; do not substitute batch start or invent them. No L3 save,
post-choice readback or clean Precision acceptance. Stale400/450 banner was not an
extension;739 clean samples/complete teardown/controls intact. Suggested next
separately granted lean replay from aaea, OMIT already-proved L2 detail scrolling,
choose/confirm/save early and fix test guard/banner rather than extend deadlines.
No product/rule/cancel-default change proposed.
Corrected minimal replay later passed clean L3 selection/save: inspected actual
`testing/mastery-l3-minimal-protocol/summary.json`. Explicit Precision141.8..142.2,
normal HUD21/28/7/14; actual named NEWEXPERT-L2-ne3 saved207.85..208.03,677850 bytes,
SHA5374a51331153f7105b93fa36799b7e85e1e28f4dfb3ed5851d5b3beb4dcffd1/read-only control.
Entry<150/choice+save<230/mandatoryQuit<300 passed. Soft250 quit target MISSED;
actual button259.460..259.636, confirmation260.017..260.194, normal exit260.346,
513 clean samples/full verified teardown. Wrong initial NEWGAME-ne3 filename
assumption and trailing post-exit identity assertion retained, not save/product
failures. Earlier late-cleanup/350 RED remains untouched. No fresh L3 readback,
effects/battle/AI/F8F9 claim. Build prepares exact tested-privateb770 default0.5.1
activation with separate guards/tests, not947 rewrite/future art/category inclusion;
Fresh L3 readback subsequently PASSED: read actual
`testing/mastery-precision-l3-readback/summary.json`: L3XP2000/ExpertArtillery+7Expert,
100Pikes/Ballista, saved Precision ACTIVE with distance/wall exemption and remaining
modifiers/restrictions, base=total21/28/7/14,last3/4/1/2,mana10/14,MP1087/2028.
Only read-only5374 input, no new save/progression/effect/AI. Actual quit168.695..168.872,
confirmation169.253..169.431, exit169.511 within target/mandatory/hard bounds,334 clean
samples and all protected candidates/maps/saves/source8 intact. Previous timing REDs
unchanged. Coherent full Windows and battle/effect/AI/other pending gates remain.
Requested explicit future-lane reopening from Build now this chain is evidenced:
separate two-trait artwork and bounded saved-detail tabs, outside activation8/947.
No edits or candidate creep before authorization; these are not full redesign completion.
Activation8 subsequently committed/pushed by Build as
413930bc32d0f8a7e56342a55084d816ae09e0d3; locally verified8 paths and prescribed
noreply author/committer. Next413930 full Windows/cloud and Linux release build/audit
are separate gates. Protected947 is not relabelled as a new binary or publication;
no Windows/effect/AI/full-goal completion inferred from activation commit.
Source planning only:
all capability/mastery details share656x108 scroll box, actual arrow/track friction
suggests future explicit Growth/Capabilities/Masteries navigation during full hero-screen
redesign. Sent Build proposal, NO product edits. Future two-icon lane also awaits
explicit reopening; no automatic permission inferred from StageA teardown.

Next convenience gates: disabled-module/portrait fallbacks, F8/F9/fresh-process and
remaining battle/AI/Windows gates; old947 remains RED historical, help-fixed947 boundedPASS;
frozen GUI button QS/QL + unavailable
states + unchanged F8/F9, actual Undead/trait graphics with descriptions, Windows/package.
No compiler/GUI checks claimed by SOURCE_READY. Offered exact42 to Build and Content;
ready to pause offline work for each new explicit quiet lease.

Actually viewed BOTH Artist native Sorcery sheets. Technical preference A meridian,
not user approval. Feedback: stronger68x51 state separation, crisp32px rank chips,
localized metal wear/creases, structured velvet folds, curved glass reflection and
richer coherent160x68 header scene. Artist reports86 exact repeated exports but
strict edge audit RED16 plus six negative rejections; concepts remain unapproved,
not imported. SUBSEQUENT USER REVIEW REJECTED BOTH as too modern/Olden Era-like;
our technical A preference is superseded, not approval. Read updated charter:
Artist alone explores three new Renaissance-like illustrative studies (study,
conjurer, manuscript), not another full family yet. No merely noisy orb/bevel
revision. User chooses before a style guide is established; original drafts and
REDs stay preserved. Artist's authorized V2 slot/retry completed; actually viewed
all three `sorcery-art/renaissance-studies-v2/{study,conjurer,manuscript}/native-review.png`
sheets. They are distinct still life/expressive hand/painted folio studies,15 samples,
not a full20-file family. Feedback sent: hard angular facets remain unfinished;
study32 needs distinction from Knowledge/book, hand anatomy/floating page needs
refinement, manuscript32 loses much celestial detail. Native header/top28 and
compact68x51 placement appear consistent, not composed GUI acceptance. Await actual
user choice/rejection; no approved style guide. Initial edge RED and later reported
geometry repair/retry0 retained. SUBSEQUENT USER REJECTED V2 as crude; all our
technical comments are historical, not approval. Read the full new
`docs/NH_SORCERY_STYLE_BRIEF.md`: miniature fantasy still-life PAINTINGS, not angular
pixel art/flat glyphs/modern jewels. Artist must first demonstrate one credible
high-resolution modeled/chiaroscuro/material-rich master and actual44/32 reductions,
not another batch/full family. Honest tool/method evidence and user visual approval
are mandatory; historical rendering claims are user references, not verified facts.
No approved motif/style guide, no parallel Sorcery authorship or live import. Existing
functional convenience/other pictograms are not retroactively accepted as finished
painting-quality art; the wider polish requirement remains open.
Artist later produced one authorized actual Blender CPU proof (reported18s/render0,
reductions0, PID gone). Actually viewed cleaned V3 `still-life-proof-v3/output/`
master-review.png and native-review.png: substantial open book, key and cloth show
real modeled volume/material/occlusion improvement; native book reads44/32. Feedback
sent: key weakens at32, regular paper/text and render grain remain quality questions.
No user approval/style guide/full family/import inferred. Raw Blender PNG metadata
remains private; cleaned-view pixel identity is a separate technical claim. Build
now owns BE-negative/restore/clean-six exclusive work; no extra render requested.
Future category DESIGN offer acknowledged (NOT API-ready): optional CreatureID
lookup on read-only world/battle callbacks, enum Core/Elite/Champion plus saved
name/description IDs and ruleset/source identity; world registry copied to BattleStart.
Requested explicit null for unmapped creatures and old-context absence, especially
NO battle fallback to current world/defaults. No out-of-game category from global
config. Need final header/signatures/fields and Build-approved mapping before UI
implementation. Explicit Conflux families/upgrades/Firebird+Phoenix entries, no
inheritance from old tier, upgrade graph or leadership weight. Metadata alone does
not change recruitment/upgrades/capacity; no fictitious separate dwelling claim.
Runtime later reports an UNREGISTERED structural category draft plus seven unexecuted
tests; enum/copy-view fields are preliminary. No GameState/serializer/callback/data
wiring or finalized CreatureID API exists yet; no Frontend code against this draft. Broader masteries, categories,
full hero-screen/art polish and outstanding earlier-family journeys still required.

## New usability authorization + Artist fence — source-only during quiet mastery GUI (historical)

User clarified F8/F9 BOTH WORK: missing buttons only. Do NOT report broken saves or
ask that question again. User identified Extras and authorized buttons/status icons.
Read updated feedback/design scope. Independently pinned Extras vcmi-1.7 metadata to
9229af99b03540df3f247dc7a570a30ef9000670: quick-button command bindings and Undead
mapping corroborated; root has no conventional license, author credits are not
permission. Bonus Icons manifest also patches creatures/spells, so blanket inclusion
would not be a reviewed presentation-only change. NO Extras art/config copied.

Build approved separate new `assets/new-horizons/generate_convenience_icons.py` and
`CONVENIENCE_ART.md`, two original24px four-state button stems NH_qsave_24/NH_qload_24
and ten original50px trait icons. Source authored with layered original book/arrows,
skull, wings, crossbow, siege wagon, shields and other pictograms; no held generator
imports or purchaser/font inputs. Syntax-only AST check passed; generation is
DEFERRED during the current quiet GUI lease. No new output/fit/quality claim yet.

Build owns targeted additive adventureMap JSON and graphics-only bonus mappings.
Proposed container top171/right69/w56/h24, childrenleft0/32, hides in world view;
minimap ends170/lists start196. Existing adventureQuickSave/Load and vcmi help keys,
playerColored=false; no whole layout overwrite or save/request bypass. Ten confirmed
bonuses: UNDEAD,FLYING,SHOOTER,SIEGE_WEAPON,NO_RETALIATION,UNLIMITED_RETALIATIONS,
TWO_HEX_ATTACK_BREATH,ATTACKS_ALL_ADJACENT,MAGIC_RESISTANCE,HP_REGENERATION. Detailed
mapping/provenance in the new note. Old421/mastery outputs, code,925 and releases
remain held/unchanged. Next after teardown: generate ONLY new38 outputs, prove prior
421 unchanged, isolated reproduction/negative controls and independent visual audit.
Do not call this ten-icon increment exhaustive polish or a legal guarantee.

Fifth worker Artist now exclusively authors Sorcery replacements in isolated
sorcery-art paths under docs/NH_ARTIST_SORCERY.md (read fully). Frontend reserves all
20 live Sorcery PNG paths for reviewed replacement but does not edit them now.
Sent Artist exact compact bookmark68x51 versus native80x60 warning, header top28
alpha/rank-size contract and selective-generator integration requirement. Await its
two native concepts/user approval/import manifest; no parallel Sorcery authorship,
no live import before approval/Content GUI. Frontend retains non-Sorcery/usability.

## Windows user feedback triage — exact891 source/ZIP, no product edits

Read docs/NH_USER_FEEDBACK.md and inspected frozen source commit
89165787e50df755ad6311365e039f3185325a09 plus actual Windows891 ZIP. Local static
report: `research/user-feedback/891-static.json` under ignored Linux build root.
Content independently corroborated its own exact-package trace.

Quicksave/load: exact packaged keys are F8/F9. AdventureMapShortcuts retains both;
F8 admission requires map view, LOCAL mode, host identity and all human connections
local; F9 additionally requires hasQuickSave. CPlayerInterface calls validated save
on SavegamePath(...,"Quicksave"), reports saving, sets hasQuickSave; F9 rechecks actual
local resource existence and server canQuickLoadGame before the confirmation/load.
No explicit quicksave/load buttons were found in shipped widget JSON. These are
static routes, NOT successful Windows execution or a proven removed/broken feature.
Need Tester's ordinary F8/file/notification/F9 confirmation/reload journey; distinguish
failed keys from missing familiar buttons and retain original/profile comparison.

Undead icon: exact ZIP config/bonuses.json UNDEAD has only creatureNature:true, no
graphics.icon/subtype/value mapping. Shipped default Necropolis Undead bonus entries
have no customIconPath; no additional shipped UNDEAD descriptor mapping found.
CStackInstance uses customIconPath if supplied, else CBonusTypeHandler's descriptor
icon; default image path therefore stays empty. CCreatureWindow explicitly omits
CPicture when that path is empty, while retaining the translated Undead description.
Essential vcmi English text describes the property; icon absence is NOT property
loss. This concretely explains the default creature-window text-without-icon path,
not the user's exact former UI pack, battlefield-marker route or upgrade history.
Required vcmi/core resources and mod loader remain; no particular omitted mod is
proven responsible. Remediation belongs in a reviewed icon provider/mapping or
licensed/reference artwork increment, not blindly changing bonus rendering/rules.

User finds provisional new medallions crude: polish remains real work, not finished
illustration. Do not rush another crude placeholder or copy an unlicensed pack.
Preserve held mastery code/art and frozen releases. Next: independent bounded
controls/creature-info route when granted, user route/version/profile clarification,
then scoped actual fix and visual-polish work outside the held mastery checkpoint.

## Actual mastery compile RED repaired — missing WindowHandler include only

Resumed combined build reached HeroMasteryWindow.cpp112 and failed on incomplete
WindowHandler. Added only `../gui/WindowHandler.h` to that CPP; no logic changes.
New SHA256 `0668821df470af5f40d21ad6d618afc282fcaefe5e2333293ed75f56c7d8bd26`.
New12-path manifest: `research/mastery-ui/source-ready-windowhandler-fixed.json`;
verified the other11 hashes unchanged. Build/Runtime/Content notified; UI/test/art
re-HOLD for Build's bounded retry. No native cases executed yet. Previous popup
source/lifecycle passes do not erase this actual compile RED or prove its repair
compiles. No frontend compiler, rules edits, GUI or891 changes.

## Covered mastery dialog defect repaired; revised SOURCE_READY independently reviewed

Content found a real source-ordering defect in initial nine-file READY: a right-click
help popup could hide the mandatory window from topWindow-only ACK/resolution routing.
Preserve that RED manifest as `research/mastery-ui/source-ready-popup-red.json`.
Fixed routing now visits all mastery windows, matches request/query IDs, latches
resolution even while covered and closes ONLY if topmost. The regular pending-dialog
pump defers subsequent prompts until covering windows disappear and safe closure
occurs; no blind pop or reentrant pop from activate(). Failure ACK under help restores
explicit selection; success request ACK alone never means completion.

Presentation transitions now live in actual shared `HeroMasteryDialogState.h`, used
by the window and the new standalone `client/tests/HeroMasteryDialogStateTest.cpp`.
Native test covers no default, immediate -1, covered failure, unrelated/late ACK,
retry, success-not-completion, wrong query, covered accepted resolution and eventual
topmost closure. PROVIDED BUT NOT COMPILED/RUN by Frontend; Build owns that gate.
`client/tests/check-mastery-dialog-routing.py` checks real source routing/closure;
ran0 and rejects two mutations restoring top-only delivery or blind close.

Exact revised12-path hashes: `research/mastery-ui/source-ready-popup-fixed.json`.
Content independently matched all12 and reran source regression0/negative controls;
its fixed-popup reports are in commands-static. Scoped diff check0. Existing seven
other UI files and12 art outputs unchanged;891 releases untouched. New production
header registration for Build: HeroMasteryDialogState.h; tests remain standalone,
not game executable sources. No native/font/GUI/query/AI/save claim from this repair.

Runtime final46-path/31-case SOURCE_READY is held; Build has combined build prepared.
Repaired Frontend READY sent; hold product files for serialized compile/native and
actual feedback. Required integrated tests still include real help-popup ACK/
resolution ordering, mandatory choices/chains/save/reload/AI and active effects.

## Mastery real UI binding SOURCE_READY — uncompiled, future only

Bound Runtime's actual APIs, not guessed names: heroGotMastery, chooseHeroMastery,
Offer/Dialog/Chosen AfterClient visitors, optional getMasteryView and saved-description
formatter. Nine owned UI files changed/new; exact SHA256 manifest and offline bounds
in `research/mastery-ui/source-ready.json` under ignored build root. New registration
for Build ONLY: `client/windows/HeroMasteryWindow.cpp` and `.h`. No CMake/rules/data
edits, compiler, GUI or891 release mutation by Frontend. Art remains accepted12 files.

New700x470 mandatory three-card window uses real saved option icons, localized names
and saved-magnitude descriptions; actual hero/skill and saved uint32 level identify
the offer. Existing configurable190x32 button resource was inspected in frozen data
(all four states). Keys1/2/3 or Select explicitly choose original offered index;
separate Confirm/Enter is disabled until a choice. No sorting/rank4/default/cancel.
Close refuses dismissal until matching QueryResolved. Positive request ID is only
queued: buttons stay blocked and window remains until authoritative completion.
Matching HeroMasteryReply failure ACK or immediate -1 clears selection and restores
explicit choices; unrelated/old ACKs cannot unblock a later request. Success ACK
alone does not close. No optimistic hero/bonus/mastery state writes.

Offer is copied before entering existing query-backed PendingDialog chain. Hero,
queryID, sequence and index go through the exact validated callback; matching query
resolution closes the window and uses existing input-settling/continuation handling.
Reviewed network interface mutex and default non-waiting human callback: ACK cannot
race GUI request-ID assignment across that mutex. No transport changes introduced.

Hero development entry also recognizes an independently saved mastery view. Readback
shows real chosen active/inactive descriptions, pending and eligible/awaiting skill
lists, never inferred from Expert or defaults. Offer/Chosen AfterClient visitors
refresh matching existing development windows AFTER game-state application. Primary/
capability-only and neither still omit absent mastery data. View wording now denotes
a displayed snapshot. Normal secondary-choice implementation and ui32 growth-level
snapshot are unchanged.

Scoped diff check0; offline card/button bounds fit. This is NOT compiled/font/scroll/
input/query/AI/save acceptance. Required oracles include explicit choice, Escape,
double-input, immediate/rejected/stale ACK recovery, accepted-state-before-close,
queued/chained levels, each effect/magnitude, saved inactive/pending/chosen/default
absence and actual human/AI journeys. Full expert-skill roster, creature categories
and further hero-screen breadth remain open beyond this first Artillery family.

Next: Build combined Runtime/UI SOURCE_READY and source HOLD/registration/serialized
compile, plus Content independent source audit. Hold these READY product files until
actual compiler/owner feedback; no self-authorized native or graphical execution.

## Mastery art independently accepted; saved-text helper reviewed; binding pending

Content independently verified exact12 additions, all421 outputs reproduced and
old409 matched BOTH frozen891 Git blobs and current files, not only our before
manifest. Independent blank/opaque/wrong-size controls reject; SVG payloads are
geometric only and motifs visually distinct. Generator/README hashes match READY.
Evidence: Tester's mastery-art-independent.json/log/script and content acceptance.
No in-game fit, query/mechanics or Windows acceptance follows from art alone.

Runtime now exposes `formatMasteryDescription(savedOption, localizedTemplate)`.
Read actual source: validates the saved option, replaces every `{magnitude}` token
from its magnitude and never consults live balance. Will reuse it rather than
introduce a second formatter. Exact callback/query/ACK/readview wiring is not READY.
Rejected replies must preserve the pending offer and re-enable explicit selection
ONLY on matching failure ACK; no default selection/dismissal. Accepted saved state
must apply before completion notice. New controls still await those real endpoints.
Build's891 Linux compile finished0; future compiler remains ungranted until combined
Runtime/UI SOURCE_READY and registration. No compiler/GUI/default or release edits.

## Next mastery family: concrete DTO/art increment READY; query binding pending

891 release remains frozen. Build reopened future source/art ownership only;
Runtime owns rules/state/query/AI, Build config/schema/CMake/metadata. Reserved owned
UI paths: HeroMasteryWindow.cpp/.h, CPlayerInterface.cpp/.h, NetPacksClient.cpp,
ClientNetPackVisitors.h as needed, plus saved readback in hero development windows.
No new CPP/H registration requested until actual wired implementation SOURCE_READY.

Runtime supplied real MasteryID/Option/Offer DTO and explicit option IDs/text/icon
keys. Effects: additional Ballista shot, no distance/wall penalties,50HP preturn
Ballista repair. Additional mandatory choice only on a level gained AFTER already
Expert, after ordinary secondary choice; never rank4/cancel/auto-default. Reply
contract hero+saved sequence+current queryID+index0..2, retain dialog until accepted
state/ack. Runtime corrected offer/reply level to uint32_t after our portability
review. Exact packet/callback/readview names still await wiring: NO guessed controls.
Reviewed existing query queue/input-settling/closeActiveLevelUpDialog lifecycle to
ensure this new window joins it rather than bypassing authority or auto-confirming.

Concrete original art now READY for Runtime-provided icon stems:
`NH_mastery_artilleryVolley`, `NH_mastery_artilleryPrecision`,
`NH_mastery_artilleryRepair`, each `_32`/`_64` PNG and editable SVG. Fan projectiles,
target sight and mechanical wrench are newly authored CC0 geometry. No text/fonts,
purchaser pixels, concept tracing or embedded content. Visually inspected contact;
all409 prior outputs unchanged and ALL421 outputs reproduced byte-identically in an
isolated temporary tree. Blank/opaque/wrong-size PNG controls reject. Current totals
200 SVG/200 PNG/21 JSON; new art is12 files, NOT UI states or finished mechanics.
Audit and exact output hashes: `research/mastery-art/audit.json` under ignored build
root; contact.png retained there. No compiler/GUI launched, no default activation.
Generator SHA `3e916cb13b11545e037d3a225f20a08715341213b6aaef31e84d25139b2000b5`;
README SHA `983979717a8d6e1f3287ee7abb5841315c53e1214da24e4bdbde23c37edd00e8`.
Scoped art diff check0. Build's translation templates must substitute `{magnitude}`
from the SAVED option DTO, not current balance/config; Precision has no amount.
Next arranged gates: independent art audit and exact wired Runtime contract, then
actual queued choice/readback implementation. No full mastery/hero-screen/category
completion, Windows build or GUI acceptance inferred from these assets.

## Actual ordinary autocombat Ballista AI PASS — bounded siege integration

Content reports normal exit0 at359.185s before450,708 samples, exact teardown and
916/map/protected originals/copies unchanged. Ordinary Gold/pursuit/manual Pikeman
defend, Options Ballista permission and normal autocombat led to actual CBattleAI
Ballista valuation on runNetwork and server SHOOT target2@100. Eight Ballista damage
events13,12,10,12,13,9,11,12 total92; AI Hold the Line then Ballista action, Pikemen
wait/move and final28 damage. Victory120XP,5 Pikemen lost,995 survived.
Evidence `testing/capability-ai-gui-59/` raw log/excerpt/screens/summary.

This is actual ordinary AI siege participation, not a scripted AI-method or
Pikemen-only proxy. It does NOT prove every AI choice, a new save/turn/transfer,
mastery/category mechanics or full redesign. Lease released; source approval below
remains the unchanged three owned files only. Await Build's integration identity/
product hold release and next real Runtime contracts; no frontend product edits.

## Capability foundation final Frontend review APPROVED — three files only

At Build's37-path `capability-integration-review/identity.json` checkpoint, compared
all three owned files byte-for-byte by SHA256 across current source, review identity
and GUI-tested cap59 identity: exact matches (2bf1e137/43cd2790/55a815f0).
Scoped diff check0. No product edits since the reviewed/compiled/GUI-tested READY.

Approved scope: CHeroWindow optional entry plus HeroGrowthWindow.cpp/.h read-only
leadership/siege extension. Saved families are queried independently, never activated
by frontend; all actual fields are retained without duplicated gameplay formulas.
Four reachable presence controls, scrolling/qualifiers, army-change/no-refund,
normal saves/reload/day2 and manual Ballista battle have bounded actual evidence
above. Hard-bound RED124 and timing/filename/audit-parser caveats remain retained.

Source portability review: standard C++ optional/string/array/widget code, no new
platform APIs, filesystem dependencies or numeric aggregate narrowing; full-width
capacity counters stay in std::to_string and primary totals remain int. Existing
client-local ui32 snapshot release repair is unchanged/outside this three-file diff.
This is portability SOURCE review, NOT a Windows build/GUI claim for capability UI.
No new artwork/proprietary bytes or frontend simulation writes were introduced.

No owned-source blocker found for this UNACTIVATED foundation checkpoint. Approval
is ONLY these three files, not all37 Runtime/Build paths, default0.4 activation,
AI-GUI acceptance, publication or full goal completion. Default module remains0.3.
Build alone stages/commits; product HOLD honored until review commit. Next arranged
wake: Build integration identity/hold release and separate Tester AI quiet lease;
mastery/categories/further hero-screen redesign remain required afterward.

## All four reachable presence states now actually GUI-evidenced

Content's ordinary same-process loads were PRIMARY-45AAE then NEITHER-LEGACY,
confirmed by runServer log, NOT the retained but unused f9 control. Primary-only
level2 retained base18/24/6/12, total20/24/6/12, last3/4/1/2, mana10/12 and
movement877/1500 with NO capability pane. Neither-family hero retained2/2/3/10,
XP0, mana95/100,15 Pikemen/9 Archers, NO development entry and original four-school
book (Magic Arrow5/Haste6/Bloodlust5). Current installed capability defaults did not
invent either saved family. Evidence `testing/capability-presence-gui-59/`.

Normal exit0 at396.893s before450,706 samples, exact teardown clean;916/map and all
protected originals/copies unchanged. No save/turn/battle in this run. Together with
prior both-feature and capability-pair-only journeys, all FOUR currently reachable
presence states have separate actual GUI evidence. No eight-fixture, broad AI,
mastery/category or full-redesign completion inferred. Lease released.

Next: Build's coherent capability checkpoint review and Runtime's subsequent real
mastery/explicit-category contracts; preserve current three READY hashes/candidates.
Further hero-screen breadth remains required, not replaced by these read-only panes.

## Actual main save reload and Blue-AI/day2 refresh PASS; timing caveat retained

Content reports actual8dc0 save reload: hero1000/town0, current688/max1170,
both primary15/20/5/10 and capability750/75%. Ordinary Blue AI turn reached Day2
with1170/1170 movement,1000 troops and gold20500->21000. This proves the observed
turn/refresh continuation, not every AI capacity or combat decision.

Exit0 at351.998s missed the requested quit-before330 target; last progress258.7s,
cleanup only afterward, original420 supervisor unchanged/no extension.645 samples,
exact teardown and916/map/all protected saves/copies unchanged. Preserve this timing
caveat rather than calling it an entirely on-target lease.

Manual distinct Day2 save actually landed at
`Saves/NHCapabilitiesArmySiege 2026-09-07 1/Autosave-111-day2.vsgm1`,576549 bytes,
SHA256 `16406d0915a32cfb5fe84caa0293f10304b8be5c7f459139681f99e517672b3c`;
readonly control retained. Name came from selected default plus typed suffix: NOT
an automatic-save claim. Evidence `testing/capability-main-reload-59/`. No Day2
restart, transfer/combat or other presence proof in this run. Lease released; next
separate gates remain owner-coordinated. No frontend source defect indicated.

## Actual cap59 transfer/movement readback and distinct save PASS

Content reports normal exit0 at468.420s before480 progress cutoff;924 samples and
exact process/socket teardown clean;916/map/protected controls unchanged.
Ordinary town travel left688 movement. Transfer500 out/back changed hero roster
1000->500->1000 and town0->500->0, total1000 preserved. Reopening development
showed movement limits1170->1560->1170 and factors75->100->75; current688 stayed
unchanged throughout. This proves actual UI readback for changed armies without
refunded remaining movement in this journey, not all AI planning behavior.

Distinct normal `profile/data/vcmi/Saves/NEWGAME-mainday1.vsgm1` saved,574828 bytes,
SHA256 `8dc0ed18869abc39ba06c33f1a3f179603e5a53eaa611b1eed4c022d80902b77`;
readonly main-day1-control copy retained. Evidence `testing/capability-transfer-gui-59/`.
Initial typing hit Filter; Tester corrected filename focus before the actual save,
retaining that test error. No next-day/reload/combat/other-presence claim. Lease
released; next reload needs separate explicit GO. No frontend repair indicated.

## Focused cap59 ordinary manual Ballista battle PASS with normal exit

Read `testing/capability-battle-gui-59/summary.json`: normal exit0 at298.346s,
588 samples, clean child/owned-INET/process/socket teardown;916/map/protected
saved controls unchanged. Six ordinary Pikeman defends and six manual Expert
Ballista target actions produced damage12,12,13,10,13,11,10,11,13,13,2 (total120).
First two shots left10 Archers with top HP6. Victory120XP,4 Pikemen lost,996
survived. Tester retained raw log SHA256
`9e92358b6654f99ce27fc3ad6d9d859769a6e5172f057dd077e244afeb0a7544`.
An initial UTF8 audit-decoder failure is retained; ASCII-byte regex audited the
unchanged log. This is not a game parser/source repair.

Prior broad main run remains RED124; this focused actual battle independently
passes its normal-input/exit scope. No transfer, new normal save/reload, other
presence state or native Windows gameplay inferred. No frontend repair requested
or indicated. Next owner-coordinated gate: army-change/current-vs-limit effects and
save/reload, remaining primary-only/neither controls as required by Tester; then
next real mastery/explicit category contracts and further hero-screen redesign.
Do not close the full goal on this capability increment or infer all AI behavior
from one manual Ballista battle. Candidate/source identities remain unchanged.

## Main cap59 both-view readback PASS; full run HARD-BOUND RED124

Content's main both-feature run hit the hard bound: exit124 at604.207s, NOT normal
quit. Exact client/Xvfb/socket/lock teardown and916/map/protected save checks passed.
Actual Gold hero15/20/5/10, XP0,1000 Pikemen, Expert Artillery/Ballista,
mana10/10 and1170/1170 movement; capacity1000/75075% and scrolled100/0/0/base-only
qualifiers were observed. No defend, Ballista shot/damage, transfer or distinct normal
save was executed/proved. Evidence: `testing/capability-main-gui-59/summary.json`.

Inspected the retained battle-intro image and client log. Image explicitly says
Press any key to start battle immediately; source has an intro-sound completion/
skip path. The last PNG predates hard termination by roughly236 seconds, so it is
NOT evidence of the screen staying frozen until timeout. Log includes active-stack
application and later music processing, not a tested battle action. No product hang
or frontend repair is established from this aborted journey; no speculative edit.

Lease released, no implicit retry/extension. Next owner-coordinated action is a
separate bounded combat/army/save grant with fresh observations and enough time for
normal teardown; preserve the existing actual GUI passes but keep action/AI/save
and remaining full redesign gates explicitly open.

## Actual capability-only save under both-feature defaults: absence preserved PASS

Content completed the separately authorized reload in unchanged cap59. Its installed
module has both primary/capability rules nonempty, but the saved hero retained
2/2/3/10, XP0,1000 Pikemen, Expert Artillery/Ballista, mana100/100 and1170/1170
movement. No growth snapshot/no saved primary profile persisted; capacity1000/750,
75%, siege100/0/0 and base-only qualifiers remained visible after scrolling.
Evidence: `testing/capability-only-reload-cap59/` summary/screens/full log.
Exit0 at331.686s (progress stopped before330, cleanup only afterward); exact process/
socket teardown, both916 inventories and all original/control/save copies unchanged.

This closes the actual capability-only saved-absence control under both-feature
installed defaults, NOT other presence combinations, turn progression, new saves,
army-change effects or combat. Lease released; next main cap59 both-view/army/combat
journey requires a separate explicit quiet GO. No implicit launch or product edits.

## Actual capability-only GUI/scroll/save creation PASS; reload still pending

Content's explicitly authorized61-authored run exited0 at463.621s; lease released,
process/socket checks clean and916 hashes/map/control inputs unchanged. Gold new
game showed authored2/2/3/10, XP0,1000 Pikemen, Expert Artillery/Ballista,
mana100/100 and movement1170/1170. Leadership readback1000/750 and75%.
Actual current-total cards correctly say No growth snapshot; no fabricated base,
class proposals or last gains. Track scrolling exposes100/0/0 control probabilities,
base-damage-only and eligible-action limitations, and No saved primary growth profile.
Inspected `testing/capability-only-gui-61-authored/04-caps-only-scrolled.png`:
those lines, cards, footer and scrollbar are readable. No owned UI defect indicated.

Normal DAY1 save `NEWGAME-caps-day1.vsgm1` was created in profile/data/vcmi/Saves/
(no scenario subfolder),435144 bytes, SHA256
`38f8b3975973e11c6c8be7b8be4664fdc0152aa320a2e33a423660eb387f1f93`;
readonly `caps-day1-control.vsgm1` retained by Tester. Save creation is NOT reload
or saved-absence proof. No battle/turn/reload accepted in this run. Next separate
explicit grant must test this save under all-cap59 and verify absent primary growth
is preserved despite installed defaults. No implicit GUI continuation, no candidate
changes. All remaining full-design/battle/chained/legacy-level gates stay open.

## Private capability candidate frozen; activated native98 green; GUI pending

Build froze `capabilities-preview-private-59` (reported916 files, client70096ce9 /
libed56ad8) with private0.4 activation and ordinary capability-map export. Independently
parsed activated XML:98 cases, failures0/errors0. Compared all three owned READY
source hashes against its BUILD-IDENTITY: exact matches. No post-copy UI changes.
This is native/identity evidence, NOT font/scroll/input or ordinary gameplay proof.

The separate unsigned snapshot repair was integrated by Build at351 with a
compile-only regression after retained red narrowing control. Build reports native
client0,59-case profiles/regressions/package gates green; corrected full Windows
run34093695275 remains pending at this checkpoint. Future capability files were
excluded from that two-file release repair. Fixed growth release stays separate.

Source HOLD released; no GUI/default activation authorized. Next arranged gate:
Content independent frozen-candidate audit, then Build's explicit quiet GUI GO.
Use actual four reachable view combinations and scroll to all siege limitations/
skill chances; retain full-design open gates. No new product changes while awaiting
concrete feedback; no Frontend compiler/GUI, no candidate mutation.

## Urgent c550 MSVC narrowing repair SOURCE READY — one header line only

Build reports Windows322 terminal client compile failure C2397 at
CPlayerInterface.cpp505: aggregate initialization narrowed ui32 hero level to int.
Changed ONLY `client/windows/GUIClasses.h::PrimaryGainSnapshot::level` from int to
ui32, matching `CGHeroInstance::level`. Header SHA256:
`dff10da82a1f3b701d17088252c9a1c6c02c4bf3e9d109317f7efbe2692464d1`.
Both arms of the sole display ternary now have the same ui32 type, losslessly
converted to `MetaString::replaceNumber(int64_t)`. Actual gains, queued capture,
secondary callbacks and serialization are unchanged; snapshot is client-local.
Scoped diff check0; NOT yet compiled. Build notified READY for bounded regression
and a changed-source full MSVC retry, not an unchanged retry. No frontend compiler,
staging or commit. Exclude all three dirty future capability UI files from this
release repair; their READY identities stay unchanged. No artifact/full Windows
build acceptance follows from this source fix. Next wake: actual Build repair gates.

## Capability client/native green; independent source review; GUI still pending

Build reports actual client build0 after Runtime fixture/AI corrections. Independently
parsed `future-capability-wait-*` XMLs and exits: each future profile58 cases,
57PASS+1skip; baseline128 with2skips, curated39 with1skip, all failures0/exit0.
This supersedes the uncompiled status below, not the missing activated/GUI gates.
No frontend product changes since the three READY hashes. Fixed c550 stays separate.

Content independently reviewed by-value optional snapshots, actual totals/no-growth
fallback, the656x108 scroll body, seven siege fields and base/control qualifications.
HeroSwitcher recreates the window, so entry visibility is reevaluated per hero.
Reviewed CTextBox's real slider creation, wrapped width reduction, line scroll step
and whole-box scroll bounds; actual scrolling/font/input are still unverified.

Important fixture scope correction: current leadership and siege getters share
`usesRules(capabilityRules)`, so FOUR actual combinations are reachable: neither,
primary-only, capability-pair-only, all. The eight-case local presence matrix is
now explicitly defensive optional handling, not eight required GUI fixtures or
proof of independent leadership-only/siege-only gameplay. No fabricated activation
will be used to force unreachable cases.

Next arranged events: Runtime ordinary fixture export, Build private0.4 activation/
native/freeze and Content offline audit/quiet GO. Source hold released but preserve
the ready product while these gates assemble. Remaining full-design and historical
unverified lifecycle gates are not closed by capability source/native green.

## Future capability UI SOURCE READY — UNCOMPILED, distinct from c550

Read Runtime's actual `getLeadershipCapacity()` and `getSiegeCapabilities()` source
contracts and implemented a read-only extension in three owned files. No art,
CMake, data, rules, activation or fixed release edits. Build explicitly released
mutable UI ownership; c550 source clones/package and Windows322 remain separate.

- Hero development entry appears if ANY real growth/leadership/siege optional view
  exists. Opening snapshots each independently. Old/c550 capability nullopt hides
  both new sections even when primary growth exists. Capability-only heroes show
  real current primary totals, not fabricated base/class/last-gain data.
- Leadership shows full-width used/capacity, actual movementPercent and authoritative
  overCapacity(). Counts include undead. Text explains no troops are removed or
  rejected by capacity alone and current remaining movement is unchanged. No tier,
  primary-rating or percentage formula is duplicated in frontend.
- Siege shows actual Artillery/Ballistics/First Aid ranks, Ballista BASE DAMAGE RANGE
  multiplier and three control probabilities. Explicitly not total damage or a
  guarantee of eligible manual action; no automatic hero-level growth claimed.
- Existing700x560 layout and close/Escape retained. Capability details and skill
  chances share the existing real scrollable656x108 CTextBox; heading explicitly
  asks to scroll. All notes/chances must be reached in actual GUI acceptance.
  Growth-only c550 layout/text remains unchanged; mastery/tier choices are absent,
  not simulated by ranks/icons. This is not the final full hero-screen redesign.

READY source SHA256:
- `client/windows/CHeroWindow.cpp`: `2bf1e1372994462cc3943a03a86cd71b9f1881197bb7347b420dd304ffb20d59`
- `client/windows/HeroGrowthWindow.cpp`: `43cd2790d13d0203e1ad191d22a1622019b821da2e1087e0af0f3564553795af`
- `client/windows/HeroGrowthWindow.h`: `55a815f02a1e3ca0b7cf5ec765bccfe422fceb2481b4384021d80946a7d3ae40`

Scoped diff check0 and offline bounds/presence matrix recorded in
`research/hero-growth-ui/capability-source-review.json` under the ignored Linux
build root. These are NOT compiled/native/font/render/scroll/input/AI acceptance.
No resource generation/compiler/GUI was run by Frontend. Next: Runtime/Build
combined SOURCE_READY and explicit HOLD, serialized compile/native checks, then a
separate frozen activated future candidate and Content quiet GUI. Required controls
include independent nullopts, cap-only hero, under/over cap and undead counts,
army split/transfer/recruit/reopen, actual skill changes, all scroll details,
base-only siege wording, save/reload and unaffected c550/legacy behavior.

## Frontend final review — growth checkpoint approved within declared scope

At Build's checkpoint request, reviewed actual owned diffs and frozen
`hero-preview-private-context/BUILD-IDENTITY.json`. **All19 owned delta hashes
match the GUI-tested frozen source exactly**; no post-freeze frontend product diff.
CMake remains Build-owned. All215 shipped Image files byte-match the candidate;
all400 earlier artwork hashes remain unchanged, with409 total SVG/PNG/JSON exports.
Final local evidence: `research/hero-growth-ui/final-owned-review.json` under the
ignored Linux build root. Scoped diff check exit0. New art is original CC0 geometry;
no purchaser/concept pixels, personal paths, credentials or gameplay state writes
were introduced in the owned product changes.

Approved owned scope: optional live-hero entry and read-only growth window;
new-scale primary help; queued four-actual-gain/level snapshot and level-up rendering
with unchanged secondary selection; nine new growth-entry art outputs and generator/
provenance docs. `client/widgets/Buttons.cpp`'s narrow two-frame disabled-checkbox
fallback was deferred from034 but IS in this tested future candidate/identity; it
may join this next checkpoint, not be silently omitted from corresponding source.
It does not alter input blocking or ordinary three/four-frame button behavior.

Independently parsed final chain XMLs/exits:36 future cases in each profile,
128/39 regressions and75 activated cases all have failures0/exit0. These complement
Content's scoped actual growth/XP/artifact/selection/save/restart/day2/legacy-entry
journeys. GUI chained/cap-zero and ordinary legacy '+1' are not silently claimed.
No frontend blocker found for this coherent growth milestone. Build alone may
stage/commit/push reviewed scope and matching tested0.3 activation; Frontend does
not commit. Published034/private candidate bytes remain untouched. Future
leadership/siege/mastery/category/further hero redesign stay OUT of this checkpoint
and remain required by the active full goal.

Next: Build checkpoint identity/hold release, then Runtime's real next-family APIs
and any concrete integration defect; no product edits while checkpoint is assembled.

## Restart/day2 and legacy no-entry controls reported PASS

Content reports actual future save restart/day2 growth continuation GREEN.
It then loaded the legacy control in the frozen future candidate: original
2/2/3/10 ratings,95/100 mana,15/9 army, no growth entry and retained four-school
book. Normal control save and exit0, hashes unchanged and lease released.
Evidence `testing/hero-gui-legacy034-context/02-original-ratings-no-growth-entry.png`;
these are Tester-reported runtime controls, not a claim Frontend launched them.
Ordinary legacy '+1' level-up, chained new levels and cap-zero GUI remain open.
Keep the shared growth source hold until Build's coherent checkpoint review; no
new feature edits or candidate mutation. Next: Build checkpoint decision and
Runtime/Content authored chained/cap/legacy-level diagnostics, followed by the
remaining actual capability/mastery/category API families.

## Actual single-level growth/selection/artifact GUI PASS; reload pending

Read Content's report and inspected
`testing/hero-gui-gold-context/11-actual-four-gain-levelup.png`: all four glyphs,
+3/+4/+1/+2, the correct level2 title, and Basic Luck versus Advanced Pathfinding
choices are readable. Actual Basic Luck selection/confirmation succeeded.
Content's subsequent growth view shows base18/24/6/12, last3/4/1/2, Total Attack20
with Axe, mana10/12 and luck1. Earlier equip/backpack/re-equip changed Total Attack
17->15->17 while Base stayed15. Both manual Start/Level2 saves were made; exit0
and frozen identity retained. No new UI fix indicated by this ordinary journey.

This is ONE level and saved-file creation, not restart, chained levels or cap-zero
acceptance. Content has a new quiet reload/old034-hero phase; shared growth sources
are explicitly held until coherent checkpoint integration, source review/docs only.
Old-hero nullopt must be checked independently of that save's four/six magic-school
context; growth absence must not reinterpret either. Next wake: actual reload and
legacy-hero result, then chained/cap diagnostics. Full remaining capabilities,
masteries, creature categories and hero-screen redesign still require real APIs
and integrated acceptance beyond this read-only growth increment.

## First actual future growth-window GUI PASS — bounded scope

Content's authorized windowed1280x800 retry exited0 and released its lease.
Inspected actual `testing/hero-gui-windowed-context/03-growth-base-vs-total.png`:
read-only entry opened/closed; four cards, footer, cap10000/divisor10 and numeric
labels are readable. Knight base15/20/5/10, class gains3/4/1/2, last gains0 and
no extra chances are shown. Starting boots produce actual Total Power6/Knowledge11
and mana11, distinct from base. No source/layout correction indicated by this run.

Tester selected Random rather than Gold; this is a fixture-control issue, not a
product defect. No actual level-up feedback, Axe, quest or save journey was proved.
Earlier bare-Xvfb fullscreen/clipping was avoided by the authorized windowed seed;
no speculative renderer fix or physical/native-Windows claim. Immutable candidate
unchanged. Next: separately authorized controlled Gold/Axe/XP/save journey, then
chained/cap-zero/old-hero controls; Runtime owns any needed authored diagnostics.
Full mastery/leadership/siege/tier/redesigned-screen scope remains unfinished.

## Private future candidate frozen — actual activation/input gates next

Build reports compiled four-gain UI,35 native GREEN and a separate private future
candidate with74 activated native passes and launcher preflight0. Source/art HOLD
is released, but candidate bytes remain immutable. Content must finish its offline
audit and receive explicit quiet GO before any GUI; no frontend compiler/GUI.
This is not yet actual growth-window/level-up acceptance or a published RC change.

Remaining full-scope API coordination sent to Runtime: real leadership/siege views,
mastery eligibility/options/validated choices and saved creature categories.
Read-only UI call-site inventory: creature details live in CStackWindow/its UnitView
inside CCreatureWindow.cpp, not a nonexistent category accessor; do not infer Core/
Elite/Champion from a legacy level. Existing commander level-up UI is a different
system, not ordinary hero masteries. Current CLevelWindow assumes a secondary-skill
rank increment; a future mastery must have a distinct real choice contract, not an
Expert skill passed through as an invalid fourth rank. No fictional bindings added.

Next wake: Content's future-candidate audit/GUI result or actual next-family Runtime
API; respond to real UI defects before unrelated breadth. Published034 and its
source/ZIP remain unchanged. Growth/leadership/siege/masteries/tier/hero-redesign
completion is not inferred from native35/74 or prior command/school acceptance.

## Future ordinary level-up feedback — four actual gains source READY

Found a concrete remaining growth UI gap: existing CLevelWindow always displayed
one legacy primary icon and '+1', even though the new authority applies four
actual deltas. Fixed only owned `client/CPlayerInterface.cpp` and
`client/windows/GUIClasses.cpp/.h`, outside034. heroGotLevel now captures actual
optional-view lastGains AND hero level by value BEFORE queuing. Runtime confirmed
GameStatePackVisitor applies levelUp(primaryGains) before this client callback;
reading later would risk a subsequent-level readback. No packet/interface/rule
change, growth prediction, or workaround for the earlier native readiness RED.

Client-local optional PrimaryGainSnapshot passes to dialog construction/update.
New heroes see all four actual signed gains, including0 at cap; queued level title
uses the captured level. Legacy nullopt retains original single-icon '+1' path.
Existing secondary-skill ordering/selection, query ID and confirmation callbacks
are unchanged. Uses already-authored32px primary glyphs; no art changes. This is
necessary ordinary-XP feedback, not a mastery-choice implementation.

Static diff check/bounds check exit0; offline rows fit before the existing skill
choice region y300. Evidence `research/hero-growth-ui/level-gains-layout.json` in
ignored Linux root; no font/render/input/compile proof yet. Current SHA256:
- CPlayerInterface.cpp `9878d497138d10ff812e095da0b787fa92abf8ce1e5fe1e533c55ae98cae8c40`
- GUIClasses.cpp `8cb9eb34063195921958b0a161b03b9ebda3c786dbec0185db5537758bb7da76`
- GUIClasses.h `50ce4256741bd3fe0d697f5ee36f4b07f70a09aee0fa2dec80b07338ade779ec`
Content independently reviewed the exact three source hashes, copied optional
snapshot before queue, non-indexing of legacy primary in the new branch, unchanged
legacy/secondary callbacks and32px row bounds within384px/beforey300. It recorded
multi-level/cap-zero/selection/base-delta/save oracles. This is source/bounds review,
not compiled/font/render/input acceptance. Independently verified earlier30-case
native profiles and7725 AI oracle do not cover this later UI change or activation.

Next: Build future compile; Content ordinary XP/secondary selection, chained levels,
zero-at-cap and legacy '+1' control on a separate activated/frozen future candidate.
Build is arranging canonical profile data/XP fixture; no034 RC merging or GUI yet.

## Future hero UI compiled; before-cap clarification READY

Independently read `future-hero-integration-repair-build.exit`:0. Registered
HeroGrowthWindow and CHeroWindow have actual compiled evidence after Runtime's
include/null-callback repairs. Parsed both future-context XMLs:29 cases each,
one failure each, both `AuthorityAppliesAndReportsAllFourActualLevelGains`.
Regression XMLs128/39 have no failures. Runtime owns the authority repair; no UI
workaround, activation or graphical acceptance inferred from this build.

After Build released HOLD, applied Runtime's queued semantic wording improvement:
HeroGrowthWindow footer and CHeroWindow entry tooltip explicitly say class gains
and extra points are proposals BEFORE the primary cap; last gains are actual.
Only two strings changed, no geometry/art/rule/API/RC changes. Diff check exit0.
Updated hashes: CHeroWindow.cpp
`67704b1ba30f973012bc7f80cd0a1d884505dc7021a107ef319f4e63fae0eb6b`,
HeroGrowthWindow.cpp
`150fe6392e96e3c7a1b5ef8a2eb317bd15aa5ed39c54529c24a6cc1fff31ce98`.
Build notified for next future incremental build, not034 refreeze. Next: Runtime
actual gain test GREEN, rebuild wording, then independently test a genuinely
activated future hero and old-hero nullopt; no new mastery/tier claims.

## Actual optional hero getter bound — future source READY, not compiled

Runtime added the real `CGHeroInstance::getPrimaryGrowthView()` declaration/body.
Bound CHeroWindow to it: only a nonempty actual saved-hero view creates the new
24x24 growth button at(273,53). New-mode class title is narrowed/shifted to avoid
overlap; legacy nullopt keeps its original title/controls. Click re-reads the
current hero's optional view before opening HeroGrowthWindow. No frontend rule
activation, HeroType profile inference or future-stat placeholders. Existing
inventory/garrison/commander/hero-switcher actions remain intact.

Growth cards now distinguish saved CLASS start from current base (level/quest
changes) and total (items/effects), show guaranteed class proposal before cap,
and show actual `lastGains` from Runtime's most recent level packet—not a future
random outcome. Existing live mana/movement/morale/luck queries retained. New-mode
primary tooltips no longer claim expanded Attack/Defense directly increase troops;
Power divisor and direct Knowledge-base-mana descriptions follow actual Runtime
source. Old-mode tooltip path unchanged. Read-only snapshot-at-opening is explicit.

Files: NEW HeroGrowthWindow.cpp/.h; CHeroWindow.cpp/.h; original generator/README,
4new24x24 entry PNGs/4editable SVGs/1 animation JSON. Existing400 art hashes unchanged;
full409 isolated regeneration byte-identical. Bounds/art evidence in ignored
`research/hero-growth-ui/{art-before,layout}.json` and
`research/hero-growth-ui/reproduce-_hdaea8c/reproduction.json`. Diff/whitespace/bounds
checks exit0; no compiler or GUI. Current hashes:
- HeroGrowthWindow.cpp `06338c2ec319d857a6f286cafa6fcb45bf89fe998159cae333f5731626529419`
- HeroGrowthWindow.h `58cc69afa5758de77fc611a5cc3bf0cc604984f6131187f2eaa27b5eaba62372`
- CHeroWindow.cpp `63cf88abfbf04cc3ca7e9d3ef032515bb0d35349e3444c887f73dad8eff8f074`
- CHeroWindow.h `30ef26425dcc8b4e2f661d15b09732256ebc8ae7f69236fcaa6dd731f20c5dfd`

Content independently audited all409 exports with isolated byte-identical
reproduction and matched all400 earlier hashes to its own accepted manifest.
Six missing/blank/duplicate/size/state/embedded-content negative controls rejected;
restored409 and legacy400 audits passed. Getter/entry/dialog source hashes,
read-only fields, nullopt gate and numeric bounds were also reviewed. Evidence:
`testing/commands-static/growth-*.json`; no compiled/font/render/input/activation
acceptance is inferred from this independent static PASS.

Runtime reviewed the actual window source: Base/Total/Class start/growth/lastGains
and four existing derived queries match its semantics, with no invented future
fields. Concrete pending wording improvement: when source HOLD lifts, explicitly
say class increments and independent+1 proposals are BEFORE the primary cap in the
footer/tooltip. Do not edit registered inputs during Build's28-case/regression run.
Runtime's detached campaign-preview null-callback guard is separate; live hero
window callbacks are unchanged. No render acceptance from semantic review.

Build notified: register the two new window files in client CMake for a FUTURE
feature build after Runtime activation/native readiness; no CMake edits by Frontend.
Immutable034/source/ZIP untouched; optional checkbox remains outside RC. Next:
Runtime semantic review, Build registration/compile, Content old-hero absence and
new-hero open/read/close, actual level-up/last-gain/item change/cap/chance feedback.
This is not native-accepted growth activation, a completed redesigned hero screen,
leadership/siege/mastery/tier implementation or graphical PASS.

## Future hero-growth view implementation — not registered or reachable yet

Runtime provided actual `newHorizonsHeroes::PrimaryGrowthView` in
`lib/entities/hero/NewHorizonsHeroRules.h`: profile starting/growth, base/modified,
independent skill chances, powerDivisor and maximumPrimary. Planned live getter
returns optional per-HERO saved view; old034 heroes must return nullopt. Getter
binding intentionally waits for Build's13-primitive checkpoint. No frontend rule
activation or template-derived profile is permitted.

Authored NEW `client/windows/HeroGrowthWindow.cpp/.h` only, outside034 and without
CMake/caller changes. Constructor accepts an actual CGHeroInstance plus that real
view type; it copies presentation values at opening and retains no hero pointer.
700x560 read-only dialog shows Total/Base/Start/Class-gain cards, independent+1
skill chances in a scrollable text box, cap/divisor and existing live mana/movement/
morale/luck queries. Uses existing original CC0 glyphs and a plain drawn panel;
no new asset bytes, leadership/siege/mastery/category placeholders or mutation.
Close/Escape returns without spending anything. This is a prepared implementation,
NOT a reachable growth feature or full redesigned hero screen acceptance.

Static diff check and offline bounds checks exit0; layout evidence at ignored
`research/hero-growth-ui/layout.json` under Linux build root. No compiler/GUI run.
Source SHA256 cpp `c0c44244ba39bc5e8aa13dfae383f0850fe58ae7ae2fec602091f862bde65098`,
header `58cc69afa5758de77fc611a5cc3bf0cc604984f6131187f2eaa27b5eaba62372`.
Next: Runtime validates exact field semantics/adds real optional getter after its
checkpoint; wire entry from live CHeroWindow only for nonempty view, then ask Build
to register/compile and Content to test actual growth/old-hero/no-mutation cases.
Do not touch pregame HeroTypeID-based CHeroOverview or immutable RC copies.

## Future live hero-view coordination; RC remains separate

User reopened future hero-screen/growth coordination while immutable034 binaries,
source and package stay fixed. Asked Runtime for real saved hero-profile/current
base-vs-modified primaries/next-level increments and explicit hero-rules activation;
leadership/siege/mastery/category views only when their mechanics exist. No local
profile formula or fictional binding will be used. Inspected CHeroOverview.h:
it is a pregame HeroTypeID template window, not the live hero instance. The live
view belongs with CHeroWindow's CGHeroInstance and must preserve equipment, army
and hero switching. Existing mana/movement/morale/luck values already have real
queries. Next feature-lane action: implement that live presentation when Runtime
supplies the integrated read-only contract; current NONE GUI quiet forbids compilers.

Build explicitly deferred the optional two-frame checkbox patch below to the NEXT
increment, outside034; no RC refreeze for that log-only warning. Dispatcher owns
its bounded PowerShell smoke repair, now handed back to Build; no competing edits
by Frontend. No new icons are counted as mastery implementation or acceptance.

## Attributed two-frame checkbox warning — bounded mutable fix READY

The added diagnostic identified historical frame0:2 warnings as
`SPRITES/lobby/checkbox`, group size2, during Content's old-save Load journey.
Inspected actual `Mods/vcmi/Content/Sprites/lobby/checkbox.json`: frame0 is Off,
frame1 On, no disabled frame. CButton::block selects BLOCKED2; ButtonBase::update
previously requested nonexistent frame2. No missing rendered pixel was isolated.

Changed only `client/widgets/Buttons.cpp`: for a BLOCKED two-frame CToggleBase,
render its actual selected frame1 or normal unchecked frame rather than frame2.
CButton still removes input events; non-toggle buttons and three/four-frame images
retain their prior behavior/diagnostics. No assets, callbacks, gameplay or frozen034
bytes changed. Diff check exit0; SHA256
`dd876e5194d21a91fbef155f2733f4dc924775bfda1127babf770550bfd4c0ee`.
Build notified for a future bounded compile/retest; inclusion in this RC is Build's
scope decision and this diagnostic-only warning must not indefinitely delay it.
No compiled or GUI fix claim yet. Retest disabled checked AND unchecked save-option
checkboxes, input blocking and absence of the attributed warning on a fresh build.

Content reports phase2 timed out124 after successful old-four-school continuation
and recruitment; new-battle NONE remains unproven. Quiet lease was released. Full
hero-family APIs still pending Runtime; no fictional frontend bindings introduced.

## Tester school-label correction

Content re-read the enlarged actual034 footer: it says CHAOS SPELLS. Earlier
"Primal" shorthand and screenshot filenames were a Tester misread, not a product
school-name defect. Treat historical Primal->All references below as Chaos->All;
actual95 failure,034 click fix, classification and cost evidence are unchanged.
No UI/data rename or candidate changes requested.

## Immutable034 actual All-click regression PASS

Read Content's durable NH_COMMAND_ACCEPTANCE record and inspected actual
`testing/magic-gui034/05-All-restored.png` and `02-real-converted-ranks.png`.
Normal school->All click restores24 first-page spells; repeated All stays selected,
pointer page2 and keyboard Right page3 work (11 final-page entries). Real new
Expert Havoc/Advanced Sorcery/Basic Light/Nature icons and labels fit the existing
hero screen. Actual Expert Implosion cost13 was cast, mana200->187,750 damage;
normal exit0. This closes the95 All-toggle defect; no further All fix is needed.
Module validation is also clean in that tested candidate. These are bounded
interaction/render/cost passes, NOT new hero growth/mastery screen acceptance.

Content now has another quiet8-minute phase for old-four-school continuation and
new-battle NONE on the unchanged immutable034 candidate. No frontend compilers,
GUI launches or candidate edits. Complete six-school keyboard, teachers/rewards,
broader effects, growth/derived attributes/masteries/hero redesign/tier presentation
and native Windows gameplay are not established by this regression. Next wake is
Content's phase2 result/defect; future hero-family wiring still needs Runtime APIs.

## Delivery pipeline checkpoint

Read NH_DELIVERY_PIPELINE.md, NH_AGENT_START.md, updated NH_WORKER_PLAN.md and
design cross-links. Existing full frontend goal is retained, not restarted.
Current release-candidate repair is the real All-toggle click defect below;
future hero-growth/mastery/tier breadth must not delay that bounded fix/retest.
Keep future feature source separate from immutable candidate bytes and report
actual Windows/Linux and GUI limits. Build alone integrates/publishes; no fifth
worker is activated and no frontend staging/commits are authorized. Arranged next
wake: Build's incremental compile/refreeze, then Content's same-path click retest.

## Actual95 All-tab click defect — local fix READY

Content's real95 GUI displayed six schools/headers and observed spell-AI Implosion
(7525 damage, mana84), but clicking All twice left the Primal/Bloodlust page.
Evidence: `testing/magic-gui95/11-All-click-stays-Primal.png` versus initial All.
This is a real frontend failure, not accepted six-school interaction.

Root cause confirmed in existing widget code: CToggleButton::clickReleased first
calls hover(false)/hover(true), THEN tests PRESSED. Our explicit setHoverable(true)
let CButton::hover replace PRESSED with HIGHLIGHTED before that check, so the
selection callback never executed. CButton defaults hoverable=false but still
registers HOVER/SHOW_POPUP; tooltips do not require hover highlighting.

Mutable `client/windows/CSpellWindow.cpp` now removes that All-toggle setting and
sets allowDeselection=false instead. CToggle's own doSelect still supplies the
selected highlight. This is local usage repair, no broad widget/rule/art change;
immutable95 remains untouched. Diff check exit0; SHA256
`f1f9e8c5856821798614e1f386a9fa3ba3619d99fa2baf77f90a9652c9d465d2`.
Immediate READY sent to Build/Content. Next: Build incremental compile/refreeze,
then actual Primal->All click, repeated All, school cycling/page/cast retest by
Content. No fixed/accepted GUI claim until that regression journey passes.

## 95a7001e3 immutable candidate; reward feedback remains authority-owned

Build released registered-source HOLD after an immutable906-file Linux95 copy
and reports113/24 native green. Content has the sole quiet10-minute GUI lease;
no frontend compiler/GUI or candidate changes. Source is at95a7001e3. Independently
read `build/new-horizons-windows-cross/sdl-main-feature-build.exit`:0, matching
Build's first feature Windows client/install success. The explicitly assigned
EntryPoint.cpp fix was exactly `#if __MINGW32__ && !defined(VCMI_SDL3)` around the
legacy `#undef main`: preserve SDL3 wrapper's SDL_main symbol, retain SDL2 behavior.
Build integrated it; Frontend made no commits. No Windows gameplay claim.

Coordinated actual reward-feedback path with Runtime: CQuestLog already passes
its game callback to quest text/components; CComponent displays the supplied
SecondarySkill ID/rank. Runtime confirmed NO new frontend API or conversion:
authored decoder, authoritative skill changes, limiter checks, reward/limiter
components and quest replacements resolve the actual skill in lib/server. Their
existing SEC_SKILL/MetaString output must be correct even for null-hero quest
previews. Do not add a second frontend remapping or alter immutable95. Runtime
will test/repair that path. Hero-family read/choice APIs remain unintegrated;
await real contracts, not fictional controls. Next: actual Tester UI defects or
new Runtime view APIs, with full growth/mastery/hero/tier scope still outstanding.

## Windows feature compilation — registered source HOLD

Build reports native113/24 gates green and is starting the first actual Windows
feature-client compile. Preserve all registered client source/headers/art during
this hold; no frontend compiler or GUI launch. Independent new files/docs are
allowed, but no real hero growth/leadership/mastery/category read-choice API exists
yet. Runtime's pure PrimaryProfile parser/math is not an integrated public view;
do not wire invented values or claim growth from that helper. Reward/limiter gaps
remain documented, so native green is not full six-school acceptance. Await Build's
actual platform result and integrated Tester gates; full redesign scope persists.

## First six-school build and bounded missing-frame diagnostic

Independently read `magic-first-build-20260906T204536Z.exit`:0. Actual log compiles
CSpellWindow.cpp at519/691 and links client at689/691. Thus saved-school UI source
now has real compiled evidence (not six-school rendered acceptance).
Parsed actual `magic-first-baseline.xml`:103 cases,1 failure; curated XML:8 cases,
1 failure. Named reds are Runtime-owned
`SuccessfulOrderDoesNotExpirePreexistingUnitTurnBonus` and
`LegacyHeaderDoesNotRequireDisablingCuratedModule`. They remain correctness gates;
no frontend bypass or weakened test. Build released source for needed owned fixes.

Read Content's actual repair66 first-journey record in NH_COMMAND_ACCEPTANCE:
chooser/cancel/target-cancel, three Orders, shared spell budget, persistent/switching
Doctrines, numeric labels/footer fitting and bookless-AI command use passed over
seven rounds. Pre/postbattle saves survived restart. Later continuation timed out124;
strong spell-AI/new-battle-NONE GUI checks remain unpassed. No broad completion.

Recurring saved-menu `unavailable frame0:2` logs still lacked a resource name.
Bounded owned diagnostic applied: `client/render/CAnimation.h` exposes immutable
resource name; `client/widgets/Images.cpp` adds that name and group frame count to
its existing failed-setFrame error. No rendering, frame selection or gameplay
behavior changes. `size(group)` inspected: const lookup only,0 if absent.
Diff check exit0. SHA256: header
`05aa2ec512e42c8a1614fd2f5ca47805cee5efdd93b8fe7d0353fce672e1cd25`, cpp
`6ba179fad22a5a12d0e349237f33bb73294f7c644b9c4998938004be02fd89b9`.
Build notified for its next compile; this diagnostic is not yet compiled and does
NOT claim to fix the unidentified missing frame. No compiler/GUI by Frontend.
Next: use actual resource-attributed logs if reproduced, respond to new UI defects,
and continue hero-family wiring when Runtime exposes real development/choice APIs.

## Original six-school skill artwork — READY for Build registration

Build explicitly authorized72 new skill PNGs plus72 editable SVGs. Added to
`assets/new-horizons/generate_icons.py`, `README.md`, owned `svg/` and mod `Images/`:
`NH_<school>Magic_<rank>_<size>.png`, school light/nature/sorcery/havoc/shadow/chaos,
rank basic/advanced/expert, size small/medium/large/scenarioBonus. Exact canvases
32x32/44x44/82x93/58x64 were read from skill schema and CSkill::registerIcons.
One/two/three lit marks express ranks1/2/3, NOT later mastery choices. Reuses our
own original CC0 geometric motifs; no purchaser/concept inputs or extracted pixels.
Build owns the six real skill definitions, gain chances and registration.

`python3 assets/new-horizons/generate_icons.py` exit0. Offline checks verify all72
RGBA dimensions/alpha, matching SVG dimensions and no embedded image/script content;
all256 prior outputs retain SHA256 exactly. Frontend inspected generated contact
pixels for every school/rank/size. Full isolated regeneration exit0: all400 files
byte-identical. Evidence under ignored Linux build root:
`research/skill-art/{before,validation}.json`, `contact.png`, and
`research/skill-art/reproduce-4gjj8tft/reproduction.json`. Total190SVG/190PNG/20JSON.
Content independently audited all400 outputs: full isolated reproduction byte-
identical, all256 previous hashes unchanged, all72 skill variants/sizes/rank markers
checked. Its missing-family and wrong-rank negative controls rejected, then restored
outputs passed. Contact pixels independently reviewed; Tester handoff contains the
record. No actual skill/mastery or graphical acceptance follows from this art PASS.
No compiler, native test or GUI launched by Frontend; frozen542 candidate untouched. Actual
skill progression, cost/rank use, hero/level-up rendering and old-save semantics
still require integrated gates. Next: independent art audit, Runtime/Build compile
readiness and school/command GUI feedback; do not equate assets with masteries.

## Actual saved-school callback wiring — awaiting Runtime/Build readiness

Runtime supplied exact game/battle classification and level APIs; inspected their
public declarations and actual definitions in `lib/spells/NewHorizonsMagic.cpp`.
CGameInfoCallback delegates game rules, BattleProxy delegates battle rules, and
CGHeroInstance uses battle-or-game saved rules for membership/level/rank/cost.
Runtime moved the game delegation from MapInfoCallback to CGameInfoCallback;
verified CCallback inherits it through CPlayerSpecificInfoCallback. This keeps
map-only editor/mock callbacks on safe legacy defaults instead of calling their
unsupported gameState(). Public signatures and frontend calls are unchanged.
Validation restricts remapped spell levels to1..5, compatible with existing level
text IDs; legacy/special-spell fallbacks remain Runtime-owned. `CSpellWindow.cpp/.h` now calls them:
`getActiveSpellSchools/getSpellSchools/getSpellLevel` in adventure context,
`battleGetActiveSpellSchools/battleGetSpellSchools/battleGetSpellLevel` in battle.
One book-local snapshot feeds sorting, learned counts, page totals, filtering and
level labels/hover. No raw CSpell school/level or global registry reads remain in
the book. Existing hero rank/best-school and cost calls are retained against
Runtime's now-present saved-context implementation. No frontend mechanics invented.

Tabs and keyboard/restored selection use only active visible IDs. New-school
order stays stable when learning spells; stale saved tabs fall back to All with
page0. Inactive legacy strip is covered by an original plain drawn panel with an
All-spells toggle reusing NH_spells_button; six custom glyphs/headers use registry
paths. Legacy four-school snapshots retain original strip/navigation. New-school
turn animation direction follows visible order rather than numeric registry IDs.
School paths/classification are data-driven; no hard-coded faction assignment.
Content independently reviewed the context/navigation and six-school geometry;
local `testing/commands-static/school-context-review.json`. Its wake described
All as48x36, but current source references NH_spells_button: Frontend decoded all
four actual64x64 frames and requested metadata correction. Exact All bounds are
(534+offR,318)..(598+offR,382), inside83x294 panel ending y382. No product change
needed. Content subsequently independently decoded all four64x64 frames, recorded
frame hashes/correct rectangles and corrected its metadata/handoff. No compiled,
rendered, cost/cast or legacy integration claim from this review.

Latest source hashes: cpp
`ceefcb46ae75ac0e3aa974cd03e778a65d26d5389dbce2ea94058c7e8424951d`,
header `9225916c6c86d57b88d97d1ab238c2e5543c132af980231a61e60783eef1bf36`.
Diff check exit0; inspected toggle silent-selection, scaled-image and color APIs.
This is NOT compiled/accepted yet: Runtime reports source WIP, with registration
and native integration still pending. Build must take the agreed shared compile
only after Runtime READY; immutable542 candidate is untouched. No art/config/CMake/rules edits. Content asked for independent source
review; active-six rendering/casts/save compatibility await coherent next freeze.

Actual first-command GUI gate FAILED activation: Tester reports fresh new game,
normal adventure save/reload and field battle opened original book rather than
chooser. BattleWindow correctly branches on authoritative battleUsesHeroCommands;
reported to Build/Runtime, no frontend force-enable or save mutation. Native fixture
overrides did not establish actual module activation. The mutable current.png had
already advanced to quit confirmation when Frontend read it; do not claim that
image independently proves the earlier book screen. Await preserved Tester record.

Next: fix any independent source-review defect, then compile with Runtime READY;
first-command activation repair/GUI retest remains necessary before accepting that
increment. Full growth/attributes/masteries/hero/tier scope remains unfinished.

## After immutable 54213f042 copy — school-context preparation

Build released source freeze after copying immutable candidate54213f042; Content
has the sole20-minute GUI lease. No frontend compiler/game launch or candidate
copy changes. Build reports95-case native gate and identity rebuild EXIT0;
actual command GUI acceptance remains pending, not inferred from those results.

Prepared `client/windows/CSpellWindow.cpp/.h` for the agreed save-scoped contract:
a single `readSchoolContext()` snapshots the existing real registry/classifications.
Sorting, custom-tab learned-spell counts, school page counts and page filtering
now share that book-local view rather than reading CSpell::schools independently.
The reader currently preserves existing semantics; there are NO fictional callback
bindings, new school IDs, global spell writes or claimed school migration. Runtime
can supply the real active IDs/classifications at this one read boundary next.
Caster school rank/best-school selection still uses existing hero mechanics;
explicitly flagged that dependency to Runtime for borders/descriptions/costs.

Static `git diff --check -- client/windows/CSpellWindow.cpp
client/windows/CSpellWindow.h` exit0. Inspection confirms direct global school reads
only inside the reader; inherited registry filtering/order semantics retained.
No compiled/runtime acceptance for this post-copy change yet. SHA256:
cpp `febe7a5551ab5f071a83e2f6880235a2be6140088427cbf2c016232f7809187f`,
header `343c429f5dd2a11894fa28c640081c44f58a0f634c64e191eb1a48816a5d31e3`.
No changes to command chooser/art/CMake/rules. Build notified to defer compiler
until quiet lease ends. Next: wire Runtime's exact callback contract, then gate
legacy/custom tab visibility, keyboard/restored selection and selected borders on
that real saved context; react immediately to candidate Tester defects.

## Current-recipient Doctrine clarification — updated chooser READY

At Tester's concrete request, exposed Runtime's declared first-slice coverage:
BOTH Orders and Doctrines affect only living ordinary own troops present when
issued, excluding war machines. Persistence across rounds does NOT grant effects
to later summons or clones. Such arrivals require switching to the other Doctrine;
reselecting the active Doctrine is invalid. No mechanics/balance changes made.

`client/battle/BattleHeroActionWindow.cpp` now states this in its visible Doctrine
caption, a two-line footer, and detailed command help; Doctrine help explicitly
explains switching and invalid same-Doctrine reselection. Existing percent values,
64px effect labels, action validation and art remain unchanged. Build notified
before freeze; updated cpp SHA256
`8da49071a6058f4a8123e04b73bc109423df464cf6ac31f49d06d1a2df3575db`.
Build reports the preceding combined build EXIT0, including chooser font fix and
school layout; combined92 native cases EXIT0 (91PASS/1 expected skip), including
both AI choices and persistence. These are Build-reported integration results,
not frontend-run tests or graphical acceptance. Final scope-clarification cpp
`8da49071...` still needs Build's next incremental compilation with the GUI exporter.
Build explicitly requests source/art frozen until a Tester defect and will send
the candidate freeze. Rendered/help-fit and command journeys remain unverified. Next executable task remains their concrete integration
feedback, then real school/hero API wiring as recorded below.

## Remaining full-scope gates and cross-owner dependencies

Full goal remains incomplete. Current source/API inspection establishes:

- Commands: bounded fixes READY; Build's next pass includes chooser font correction
  and school layout. Previous native run still had one AI spell-choice failure;
  Runtime is correcting its fixture/oracle. No frozen command GUI acceptance yet.
- Runtime confirmed next-family direction: retain four builtin school IDs and
  register six new IDs; expose save-scoped active IDs AND per-spell classification
  through game/battle callbacks. Do not overwrite global `CSpell::schools`, which
  would reinterpret old saves. Exact public API follows after the first gate;
  no frozen translation units/API edits are requested during command acceptance.
  Frontend must route book filtering/page counts/school borders through that
  classification contract, not merely change visible tabs.
- Schools: registry supplies IDs, scope, names and resource paths. Generic layout,
  ID-based filtering/casting and artwork are ready; need Runtime's game/save-scoped
  active-school list for BOTH battle and adventure books before removing old tabs
  or assigning a fixed six-school navigation order. Installed art is not ruleset
  identity. No faction table invented.
- Hero screen: inspected CHeroWindow; live primary values, manaLimit, morale/luck,
  class, inventory, army and ordinary secondary skills already have real backing.
  Preserve its artifact/army/switcher controls. Runtime must expose the actual
  deterministic growth profile, leadership/siege attributes, mastery eligibility/
  choices and creature categories before those new values/actions can be wired.
  Do not infer masteries from ordinary Expert skill level, creature category from
  legacy numeric tier, or capacity from an invented frontend formula. Read/choice
  API coordination requested directly from Runtime; no cross-owner code edits.
- Art: original command/school assets plus all15 hero motifs have independent
  static provenance/dimension/reproduction PASS. Later hero/control rendering and
  runtime behavior still need integrated Tester evidence; assets alone are not
  completion of any missing gameplay family.

Build/Runtime have explicit wake requests for compiler failures, candidate/Tester
results and next-family APIs. First complete the integrated command gate; then wire
actual school identity and the hero development presentation/choices. No commits,
GUI launches, architecture expansion or rule/CMake edits by Frontend.

## Custom-school layout implementation — ready for Build

Changed only `client/windows/CSpellWindow.cpp` after the command/art freeze.
Existing custom-school book code overlapped80x60 glyphs when more than five
schools were shown in a small book (six in a large book); its truncated hit rows
also disagreed with the selected glyph moved to foreground. Now excess custom
bookmarks use the existing aspect-preserving CAnimImage Rect constructor to fit
inside the same reserved strip, without overlap. Six small-book bookmarks become
68x51; hit areas use the actual rendered image rectangle. At or below the normal
capacity, positions and dimensions remain unchanged. No legacy tabs, spell
classification, costs, targets or save state are changed. Existing authoritative
cast paths and school name/help lookup are retained. This is a real six-school
layout prerequisite, not a completed six-school rules/content migration.

Static validation: `git diff --check -- client/windows/CSpellWindow.cpp` exit0.
Offline geometry checks extracted source constants and covered all24 small/large
count cases (0..10/0..12), verifying bounds, no overlap, positive dimensions and
unchanged full-size layouts for the authored80x60 bookmark contract. Evidence:
ignored `research/spellbook-layout/geometry.json` under the Linux build root.
SHA256 `743808177cc6c69bd5f8a7151c3aa35c9afa09a36b18dedfdbefb40249c4f573`.
Content subsequently independently read the source and CAnimImage Rect constructor
and checked all24 geometry cases: PASS recorded in `NH_COMMAND_ACCEPTANCE.md`,
with local `testing/commands-static/school-layout-independent.json`. This confirms
the geometry review only, not an active registry or rendered hit testing.
Build must compile; Tester must exercise six actual registered schools, mouse and
keyboard selection, headers/pages/search and casts after coherent registry freeze.
No graphical PASS claimed. New hero art independently reproduced all256 outputs
by Content; its evidence is `testing/commands-static/hero-art-audit.json`.

Next: respond to integrated command/AI/GUI defects; then wire stable active-school
navigation when Runtime provides save-scoped school identity. Generic layout no
longer depends on waiting for that API. Hero growth/mastery/tier APIs and screen
remain unfinished; original display glyphs are available but not fake controls.

## Follow-up: font-fit correction and hero-glyph preparation

Tester supplied actual external SMALFONT metrics (offline, not GUI): line height
16px, previous physical-damage line166px versus width163px. Corrected chooser
numeric caption to `Physical taken +/-N%` (full tooltip still states physical
**damage taken**), and expanded Doctrine labels from47px to64px height, y394..458,
before footer y463. This accommodates four bitmap-font lines rather than clipping
three48px lines. Build notified to incrementally rebuild before freeze.
Updated cpp SHA256 `0b85df8fc755d523b8b529ca6a25f5e90e5002b953994a32581e1f5147318e55`;
header unchanged. Actual font/render/input verification remains Tester-owned.

Added 15 original display motifs in two sizes (32/64): four primaries, mana,
leadership, movement, morale, luck, siege, growth, mastery, Core/Elite/Champion.
Files: `assets/new-horizons/generate_icons.py`, `README.md`, 30 new SVGs and 30
new PNGs `NH_hero_<id>_<size>` under owned source/Images directories. No fake
controls, attribute formulas, classifications or mastery choices were added.
They share the original CC0 geometric provenance and provisional-style declaration.

Validation: `python3 assets/new-horizons/generate_icons.py` exit0. Offline Python
checks verified all196 prior outputs SHA-identical, 30 new RGBA dimensions/alpha,
matching SVG dimensions and no embedded image/script/foreignObject elements.
Evidence: ignored `research/hero-art/{before,validation}.json` and `contact.png`
under the Linux build root. Frontend inspected the actual generated contact sheet;
this is art review, not in-game acceptance. Full exports now118 SVG/118 PNG/20 JSON.
Build authorized new art while existing command sources were otherwise frozen.
Additional isolated reproduction exit0: all256 outputs byte-identical using a
copied generator; no product outputs touched. Full hashes and generator identity:
`research/hero-art/reproduce-a6rev_be/reproduction.json` under the same ignored root.

Independent schoolbook audit: current registry offers `getAllObjects`, IDs/scope,
header/bookmark paths; existing casting/search/page code already uses school IDs.
But legacy tabs always remain, custom tabs reorder by learned-spell count, and no
save-scoped active-school API is present. Asked Runtime/Build for actual next-family
IDs and active-school identity for adventure AND battle books. Do not infer game
rules from installed art or fabricate a completed migration. Next: fix any command
compile/Tester defect and integrate stable school navigation once that contract is
available; hero glyphs are preparation, not full hero-screen completion.

## Post-reboot chooser correction — ready for integrated rebuild

Read `NH_WORKER_PLAN.md`; full frontend scope remains commands, six-school book,
hero growth/attributes/masteries/tier presentation and hero-screen redesign.
First-command readiness is not full-scope completion. Sole Build compiles; sole
Content Tester launches graphical journeys. No commits or cross-owner edits.

Changed only `client/battle/BattleHeroActionWindow.cpp/.h` in this checkpoint:

- Corrected Aggressive's tooltip to include **both melee and ranged** damage,
  matching current `config/newHorizonsCombat.json`; Waiting remains allowed.
- Visible effect summaries now read the saved battle rules through existing
  `heroCommands::bonuses`, using the current hero's Attack/Defense. They show
  actual rounded/capped percent bonuses, physical damage-taken penalties and
  base-speed changes rather than duplicating coefficients in the frontend.
  Read-only bonus values are never installed or sent as gameplay mutations.
- Detailed tooltips retain duration, provisional Hold-the-Line scope, shared
  action/no-mana information. Cache numeric descriptions by hero ratings within
  the immutable battle-rules snapshot; authoritative availability still refreshes.
- Avoid calling CLabel::setText on unchanged status: it unconditionally requests
  parent redraw, and this chooser checks status from show(). Button::block already
  protects unchanged state; preserve that existing behavior.
- Preserved Dispatcher-added `gui/Shortcut.h` and existing weak battle ownership,
  click-time validation, cancellation and authoritative request path.

Static check: `git diff --check -- client/battle/BattleHeroActionWindow.cpp
client/battle/BattleHeroActionWindow.h` exit 0 (untracked files also inspected).
Source SHA256: cpp `805704465874d3001524fde843c2b0a441c35e066aa4c0ac0040da78a21547b2`,
header `7d22543e35267d6d6dbc928aae7f9dd5789dc0e1f6e71e2b90fd494ada24e322`.
No compile or graphical PASS claimed for this change; Build's current native lane
must incrementally rebuild it before freeze. Tester must check numeric-label
fitting (especially Aggressive's three effects), penalties and actual commands.
Art unchanged here; earlier padding reproduction evidence is historical until
Tester verifies the current frozen assets. Build corrected its mod mount path.

Next executable task: address any integrated compiler/Tester defect, then audit
existing custom-school navigation/layout against all six registered schools and
coordinate actual IDs with Runtime/Build before wiring further book controls.


Status: two-file implementation authorized and applied; compile and runtime
verification pending. Original proposal below is retained as the scope record;
implementation details and coordination updates follow.
Inspected source: `a9b6d945e`; initial `git status --short` was empty.
Scope: this separate New Horizons fork only, not Reconstruction.

Read before planning: `AGENTS.md`, `docs/NEW_HORIZONS_MVP.md`, and upstream
`docs/developers/{Coding_Guidelines,Code_Structure,Networking,Serialization}.md`.
The Networking document's single-player TCP statement is historical: actual
source already has an internal connection. The MVP contract takes precedence.

## Exact proposed W2 source files

1. `client/CServerHandler.cpp`
   - Make local single-player startup choose `ServerThreadRunner` regardless of
     persisted `server.useProcess`. Cover NONE (new scenario/tutorial/campaign
     setup), SINGLE, CAMPAIGN and TUTORIAL load modes, not just SINGLE.
   - Preserve the multiplayer implementation as unreachable legacy machinery;
     do not rewrite server lifetime or remove process-runner classes here.
   - Remove the single-player debug start/load escape through
     `session.donotstartserver`; retain normal request/validation flow.
2. `client/mainmenu/CMainMenu.cpp`
   - Do not construct menu buttons for parsed `start multi` / `load multi`
     commands; this also removes their registered keyboard shortcuts. Keep the
     existing positions/art/resources of remaining buttons, rather than
     redesigning the menu or editing owned-by-W3 JSON.
   - Guard `openLobby` before resetting state against guest/remote, MULTI and
     hotseat requests. This is an unsupported-entry policy, not removal of
     networking facilities or a source-modification restriction.
   - For local single-player, `CSimpleJoinScreen` must start locally even with
     stale `session.donotstartserver`; do not expose editable address/port or a
     second connect action in that path. Keep progress, Cancel, and existing
     connection/failure callbacks. Preserve legacy multiplayer dialog code.

No header/API change proposed. No `client/lobby/` edits proposed for this first
patch: scenario/campaign selection, save filters, random-map setup, difficulty,
options and start validation remain usable as-is. No `ServerRunner*`, server,
lib, build, configuration, launcher or global-lobby source edits by W2.
This document is the specifically requested documentation exception to W2's
source ownership. Coordinate before enlarging the file list.

## Actual start/load trace

- `CMainMenu.cpp::genCommand`: `start single` calls
  `openLobby(newGame, true, {}, NONE, false)`; `load single` calls
  `openLobby(loadGame, true, {}, SINGLE, false)`. Campaign/tutorial loads use
  CAMPAIGN/TUTORIAL respectively.
- `openLobby` calls `resetStateForLobby` with NEW_GAME or LOAD_GAME and LOCAL,
  sets load/hotseat/battle flags, then constructs `CSimpleJoinScreen`.
- `CSimpleJoinScreen` normally calls `startConnection()` for a host. Empty
  address calls `CServerHandler::startLocalServerAndConnect(false)`.
  Currently `session.donotstartserver` instead exposes remote address entry.
- `startLocalServerAndConnect` currently honors `server.useProcess` on desktop.
  It supplies last difficulty in a fresh StartInfo, then calls
  `runner.start(loadMode == MULTI, connectToLobby, si)` and `connectToServer`.
- `connectToServer` selects the runner when `isServerLocal()` (runner != null).
  Hostname/port arguments alone do not imply a socket in this branch.
- `ServerThreadRunner::start` creates `CVCMIServer`, starts `runServer`, calls
  `prepare(false, false)` for single-player and waits for readiness.
  `CVCMIServer::startAcceptingIncomingConnections(false)` creates a network
  server wrapper but does not call its `start(port)` listener operation.
- `ServerThreadRunner::connect`, with lobbyMode false, calls
  `INetworkHandler::createInternalConnection`. `NetworkHandler` constructs
  `InternalConnection`, hands it to `receiveInternalConnection`, then posts
  the client connection-established callback to the existing event context.
- `CLobbyScreen::startScenario` calls `validateGameStart`, then `sendStartGame`:
  LobbyPrepareStartGame and LobbyStartGame still pass through the connection.
  `startGameplay` dispatches NEW_GAME/CAMPAIGN to client new-game setup and
  LOAD_GAME to `client->loadGame(gameState)`; frontend must not deserialize or
  mutate authoritative gameplay directly as a substitute.
- `openCampaignLobby` also uses `CSimpleJoinScreen`, with campaign state queued
  for sending. Tutorial uses ordinary new-game lobby plus
  `startMapAfterConnection`. Preserve these routes and campaign continuation.
- `debugStartTest(filename, save)` uses NEW_GAME/LOAD_GAME setup but currently
  has its own `donotstartserver` branch; include it in transport-policy review.

## Runtime interface agreement requested from W1

Keep existing `IServerRunner` signatures:

```cpp
void start(bool listenForConnections, bool connectToLobby,
           std::shared_ptr<StartInfo> startingInfo);
void connect(INetworkHandler & network, INetworkClientListener & listener);
void shutdown();
void wait();
int exitCode();
```

W2 single-player contract: construct a thread runner; call
`start(false, false, startingInfo)` (the existing loadMode predicate evaluates
false for all supported single-player entries); then call `connect` through
CServerHandler. No process or TCP fallback on internal-start failure. No new
transport, direct game-state channel, or serialization version change.

W1 owns readiness exception propagation, partial-start cleanup and lifetime
inside `ServerRunner*`/simulation. Please ensure start either reports readiness
or a catchable failure, never an unresolved readiness wait. Agree the exception
behavior before adding frontend error recovery; W2 should reuse the existing
error/cancel UI rather than guess a new asynchronous runner API.

Preserve lifecycle: `sendClientDisconnecting` sends LobbyClientDisconnected
with shutdownServer for local sessions; cancellation sets CONNECTION_CANCELLED
and requests runner shutdown; `waitForServerShutdown` handles joining/reset.
Do not bypass these by directly destroying a running simulation. W1/W5 should
review cancellation-before-connection and failure-before-ready independently.

## Curated UI and content boundary

Retain New/Load single-player, original campaigns and tutorial, save/reload,
scenario setup, settings, credits, high scores and exit. Do not delete art,
translations, manifests, dependency loaders or resources labeled `vcmi`/mod:
these are engine infrastructure, not automatically optional content.

No optional-mod installation/selection command was found in the inspected main
menu command dispatcher. Hiding multiplayer here is not sufficient to implement
the complete curated-content policy. W3/integrator must own the allowed content
inventory, mainmenu/campaign configuration, persisted optional-mod handling,
and launcher/package entry policy. Preserve dependency incompatibility errors;
do not silently activate missing mods to load a map/save or hide errors.
Do not blacklist arbitrary map filenames/extensions as a substitute for that
inventory. Battle-only and extra-rule UI policy should be agreed with W3 before
removal; this initial proposal preserves them rather than risking original
scenario/campaign play. Global-lobby initialization, external launch arguments
and entry points outside these owned files need separate owner review; W2's
menu guard alone is not an application-wide no-network proof.

## Validation and coordination

Before implementation, agree this file boundary and runner failure behavior
with W1; coordinate content/UI decisions with W3 and save continuity with W4.
W5 negative cases: persisted useProcess=true; donotstartserver=true; new, load,
campaign and tutorial modes; alternate multiplayer commands/shortcuts; cancel
while connecting; failed prepare; repeated start/quit/reload. Verify callbacks,
packet validation and presentation ordering remain intact.

No assigned build path was supplied to W2, so no build root was created or
build attempted. Use only the integrator/W6-assigned existing build for later
compile checks. No GUI/game launch, package installation, commit or push was
performed. Source inspection cannot establish playable acceptance or absence
of runtime sockets/children. The full MVP play journey requires a separately
authorized bounded run and independent process/socket observation.

## Authorized implementation update

Only `client/CServerHandler.cpp` and `client/mainmenu/CMainMenu.cpp` were edited
as product source. Persisted process selection is now restricted to MULTI;
debug start/load always starts locally. Main menu skips multiplayer button
construction (including shortcuts), and openLobby rejects remote/guest/MULTI/
hotseat arguments before state mutation.

The single-player CSimpleJoinScreen branch reuses built-in `loadbar` artwork
and the existing Cancel button. It constructs no address/port fields, Connect
button or connection/server title; ignores donotstartserver; immediately starts
local setup; and retains the class identity expected by lobby callbacks. This
is a transient loading surface, not a host/join choice. Normal scenario/options
and save-selection screens, Begin/Load buttons and gameplay progress are
unchanged. Existing MUDIALOG artwork has address-related content, so it is not
used for single-player. The nullable title is checked on cancellation.

Cancellation can race the posted internal-connection callback. The callback
now checks cancellation under the interface mutex before its CONNECTING assert,
closes the abandoned connection and joins through waitForServerShutdown. Queued
lobby packets are ignored after cancellation; a cancelled established session
no longer surfaces an unexpected-disconnection dialog.

### Runtime contract response

Read Runtime's updated readiness/lifetime contract during implementation.
CServerHandler catches failed start, resets the safely destructible runner,
restores NONE and rethrows; it never connects or falls back after failure.
The shared menu helper catches std::exception outside progress-window
construction and reports the existing localized unable-start-map/reason dialog
with the original diagnostic. Thus a constructor-time failure cannot push a
progress window above its error dialog. Campaign setup uses the same helper.
Unknown exceptions continue to propagate, matching Runtime's contract. Debug
startup failures also propagate rather than waiting for an unscheduled callback.

Runtime retains ownership of startup promise propagation, safe destructor/
shutdown/wait and synchronous preparation. Frontend still releases the GUI
mutex when joining through the existing helper. Neither change establishes
concurrent start/reset safety; rapid cancel/re-enter and repeated session tests
remain required.

### Build owner request and evidence

W6/integrator: please compile the changed CServerHandler.cpp and
mainmenu/CMainMenu.cpp in the active `build/new-horizons-linux` build after
Runtime's changes are included. W2 did not start a competing build.

`git diff --check` on both source files passed. Inline Python source-contract
checks passed for process-selection gating, removal of the debug escape, local
progress branch without address/connect/title controls, multiplayer guard and
button filtering, and cancelled callback/packet guards. Additional source
checks verify failed preparation resets/rethrows before connect and the menu
helper reports errors outside constructor execution. These checks are not C++
compilation, unit execution or graphical acceptance.

### Actual remaining UI/validation limits

- Loading artwork and Cancel placement have not been rendered; installed-asset
  visual verification is still needed. The setup surface is static artwork,
  not a fabricated numerical progress indicator. Existing gameplay loading
  progress remains intact.
- Runner start is synchronous: Cancel cannot be processed during preparation
  itself. It is available once control returns while handshake/setup completes.
- Scenario/options retain battle-only, extra options and random-map controls;
  content/extra-rule curation remains W3/integrator work, not deleted resources.
- Ordinary setup no longer displays the join/address screen. Legacy remote
  dialogs and global-lobby code still exist outside reachable menu entries;
  this is not an application-wide no-network proof.
- Existing unexpected-disconnection and compatibility error diagnostics may
  still use upstream terminology. No new translations or configuration edits
  were made; engine mod/dependency validation was not bypassed.
- No game/GUI launch, package installation, commit or push. Other workers'
  runtime/server/build changes were preserved. Full MVP play and negative
  failure/cancel/reload tests remain pending authorized execution.

## Independent runtime/client teardown review (follow-up)

Inspected the actual pending ServerRunner and CVCMIServer diffs against
NetworkHandler::createInternalConnection, InternalConnection::{close,disconnect},
NetworkServer::receiveInternalConnection and the client callbacks. No Runtime
files were edited.

Concrete findings communicated to Runtime/integrator:

1. `stop()`/Asio stop plus final SHUTDOWN does not call the client's
   onDisconnected. InternalConnection destruction likewise does not emit that
   callback. Our earlier frontend Cancel closed the window immediately and,
   after onConnectionEstablished had already run, had no guaranteed join/reset
   trigger. This is a frontend cleanup defect, not a request for Runtime to
   synthesize network events.
2. Early Cancel also allowed a new setup while the previous readiness callback
   was queued. Checking only CONNECTION_CANCELLED was insufficient once a new
   reset changed the state back to CONNECTING. Runner destruction while holding
   the GUI mutex is not a safe replacement for orderly serialized teardown.
3. A successful synchronous start does not guarantee successful connection
   allocation/posting. The earlier try/catch covered prepare only, leaving a
   live worker if connectToServer threw during progress-window construction.
4. Queued packet callbacks carried an explicit connection identity, but the
   frontend discarded it. After reset that could feed a previous session's
   packet into the new logicConnection or a null connection.

Own-file fixes now applied:

- Local cancellation schedules the existing network timer, even when the
  internal transport never emits a disconnection event. Cancel is disabled and
  the same loading surface stays up until cleanup is complete; no host/join UI.
- A cancelled readiness callback records its connection identity and closes it.
  If the timer happens to arrive first, it reschedules until that already-posted
  internal callback has been consumed. No new setup is exposed in the meantime.
- The timer closes/reset connections and pending tutorial auto-start, joins via
  waitForServerShutdown (releasing GUI mutex), then dismisses the loading surface
  and returns to NONE. It tolerates an already-joined runner. Obsolete retry
  timers outside CONNECTING do not reconnect/assert.
- Cancelled onDisconnected retains identity until timer cleanup. Packet callbacks
  reject mismatched connections. Connection-failed callbacks check cancellation
  under the mutex, before asserting CONNECTING.
- Failure after successful readiness requests shutdown and joins before
  propagating to the existing local-setup error dialog; no fallback or retry.

Runtime's readiness promise ownership, joined preparation exception rethrow,
thread-creation failure cleanup and stopped-before-run semantics appear coherent
with these callers by source inspection. `run()` exceptions still terminate the
worker/process as documented; not reclassified as preparation failures. Raw
stop is cancellation, not graceful gameplay disconnect: keep the ordinary
packet-driven sendClientDisconnecting path for game exit. Runtime must retain
shutdown/wait safety after failed start and must not assume stopping alone has
completed client cleanup.

Build owner: these two frontend files changed again during the combined build;
please rebuild their objects after this follow-up. No competing build was run.
Need independent runtime cases for cancellation before callback, after callback
but before lobby acknowledgement, rapid cancel/re-enter, preparation failure,
connection setup failure, and normal exit/reload. Source reasoning is not a
replacement for these tests or graphical acceptance.
