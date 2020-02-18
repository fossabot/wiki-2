# 3.3. Needed Patches
In addition to cerata, several patches are also required. These patches correct
any mistakes in the cerata that should be fixed by the maintainer. The patches
also make small modifications to make the cerata easier to work with.

!!! warning
    The following patches are required to construct and envenomate the final
    system glaucus. They are automatically fetched and applied.

!!! note
    These patches are neither applied to the toolchain nor to the chroot
    environment.

## 3.3.1. attr
### 3.3.1.1. 0001-test-escape-left-brace-in-a-regex-in-test-run.patch
Source: upstream

Size: 777B

SHA-512 Sum: 1ec29779355de6b75371b383b76a1a07c625f11361b84a9e09287bcd16d5f0a1a
be02a57201d94a32929921596ebd1893882d0c52cb6d75170ae625761e9082b

### 3.3.1.1. 0002-man-fix-bold-style-in-SEE-ALSO-section.patch
Source: upstream

Size: 3.2K

SHA-512 Sum: 3925fb7d51e0e5aa67d7524da4490f13b80898841cece2864cba88dc2af416bb1
61ae9c89e7eb70d25b699cee8930a3de908c9ac3ef609e4ac91b0e516d686bc

### 3.3.1.1. 0003-man-standardize-AUTHORS-section.patch
Source: upstream

Size: 1.9K

SHA-512 Sum: 4ba931e04f8b266c9cd6d7ebde72f23e4e3e12da148ea1f06439983cfa03b6ecc
cf34eb7b7653d6cadba341e4194d97f089909573b71dd4d703e67c33e05aad0

### 3.3.1.1. 0005-getfattr.1-by-default-only-user-namespace-attributes.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 40caa7d180c0e62d76324e8a3c7ca79b9bd2d6c41b331eaabafcc0ca2f70394fe
fb1d39cd1dee2728d3ca7a4ca02b67d834a49c91eccfb3612edeefd6eb7f9fa

### 3.3.1.1. 0006-attr_list.3-Fix-the-attributes.h-include-path.patch
Source: upstream

Size: 878B

SHA-512 Sum: 4cad91f497d62d64af127dd7fd916ffa874789f678ade43ee8cf03a48a13c66f0
41cc6a8a882f80735d4785f02d223c94f853cb503462f14ae2b785159fdc253

### 3.3.1.1. 0007-Switch-back-to-syscall.patch
Source: upstream

Size: 3.8K

SHA-512 Sum: a410d9ada3c70deb24a9f4f569013f00d9b817e2c02df474d6af0ab5102db3d80
bf6d6934a9d1a1fb5f03ecc5f1869a8c6bed2bdd56f13d19ee6c38be341ebfb

### 3.3.1.1. 0008-attr_multi-attr_multif-Don-t-set-errno-to-EINVAL.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: 88936c7f229699bcd22269b7d99382e8c301e413b0f9600fa2cceb9e14b1c725f
107dc36ebd8a2d378bd2466d8835229ac26f6836e3590229a2d4f10a0f7b8c4

### 3.3.1.1. 0009-attr_list-attr_listf-Guard-against-unterminated-buff.patch
Source: upstream

Size: 2.1K

SHA-512 Sum: 6f00d997bbff3096cb0cc8a4f96e5fdc9fdb4f1e5e48043af415382fd4ee59c28
a30f4fd2d362a6f45cc1208e06ac9f1e401120adccc3b30587d75c28c384ee2

### 3.3.1.1. 0010-getfattr-don-t-count-terminating-NULL-in-well_enough.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: 55d787a51098e94f628d91b76285da5567348011c7c8acac8bad532a60fad3d92
7a4dffc825b87aea13e4846a42f578624ff69f02543425be1dbe84e47b31564

### 3.3.1.1. 0011-attr-Replace-bzero-with-memset.patch
Source: upstream

Size: 2.3K

SHA-512 Sum: ab09ae16e1d6cd445469c3e9d4d4839c365c1b4789bc5d28af2da70129f21cdee
65bf270a672fa63fe2c0769b7ddbfca2e424eb91746ab3a88f9fbdfa8e0443b

## 3.3.2. autoconf
### 3.3.2.1. autoconf-2.69-fix-perl-regex.patch
Source: alpine

Size: 342B

SHA-512 Sum: 8b779ecec178091c899b75df4471fb72334a062d6b413502d414e8827fe0c9e2f
335a8bef6878ae261e1af1568e3fe71fe82d6b5e53cb54e6585ffd91f069d8d

## 3.3.3. automake
### 3.3.3.1. 0002-bin-Rely-only-on-the-shebang-line.patch
Source: upstream

Size: 1.8K

SHA-512 Sum: 26d2941e8f8037edfafb6b408b9032994e53edee7b608c2fd7781a0153962c778
2f302536fa29d0752a2ffe00627a41fc4b3ef2640a144275a1225ead5e02c4b

### 3.3.3.1. 0007-python-Don-t-use-n-in-sed-substitution.patch
Source: upstream

Size: 1.4K

SHA-512 Sum: b686d3b461fedcbe9cb3fcb085977a6f22f9fe4c3d54fc597ff8a28801f73d172
280272bf5098f63898ba64db96c4dda10a92c00c111a5516167710a40d90800

### 3.3.3.1. 0008-doc-Fix-various-typos-and-phrasing.patch
Source: upstream

Size: 67K

SHA-512 Sum: 1a5990827966717ce1d1ec74a7738ab0c60f283da5494c3b619e38e808b104ac2
e5c7eabd457a784231bfe5c3bf51f76bd8c38b75651f138eb9e9bcf29644f04

### 3.3.3.1. 0009-ar-lib-Fix-for-MSVC-14.patch
Source: upstream

Size: 1.2K

SHA-512 Sum: 5a19b1bd549c411229902ea4c4a952867319717ee0f891e1f67c22357cecebc63
5d8ea512e6d127d9ffedeb58497abc22b456260a7ee04e36052fca739964570

### 3.3.3.1. 0010-install-sh-support-s-with-read-only-source.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: f925b23238299b8ed7e6dd8210c24bd34aee3424e463c63dd382e45a3567284a1
a78a6570a184ab98903de72136ace052fab38687644485cc0e245ecec31fa46

### 3.3.3.1. 0012-maint-make-fetch.patch
Source: upstream

Size: 173K

SHA-512 Sum: b9f1403752a9bd044a7e1f4f7ab55e2a952ce664780f0c86057da1805545094b0
39317bfe786fb6a86aac10b33c299eebcbc91200e02d4b78aea46630b18c9eb

### 3.3.3.1. 0014-config-add-msys-support.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: dfa91d303d37ac1d565d1d3fd6469efc409a0c0ee17c1cf786be296192c9c3bb2
e8aad54e6fe917b161d15e9f90635cb1ca78de222b59b18a925a6e899d08b1c

### 3.3.3.1. 0015-dist-add-dist-zstd-option.patch
Source: upstream

Size: 7.0K

SHA-512 Sum: 81130e65768c4b0c28ad2e8448a44f5414943bb08618bf323c2a2d573478a66b8
f566a14b191bdea5e748e4f128a12e611a54aa55515bc3a5ff9b05fc71aa805

### 3.3.3.1. 0018-maint-make-maintainer-check-tests-pass.patch
Source: upstream

Size: 1.7K

SHA-512 Sum: 8ac61afd0d99cab35a566d5d45e2b4f933c1fd53f2e523889497b107b01c0a6a6
db22e3ecb6dc020c915b8228afb395f73f0bcf046c0dc021ab4a0591fb7799f

### 3.3.3.1. 0020-automake-Support-byte-compilation-in-older-Emacsen.patch
Source: upstream

Size: 3.4K

SHA-512 Sum: cdef633cec51ad5885a696d99f83c1d75234e5209f90c8afb15db345d5ff8bbaf
91f538201e49521cfd4247b793ec9a44c86a100b089a282ab3d0c6c4e4f7623

### 3.3.3.1. 0021-tests-Correctly-simulate-no-emacs-in-t-nobase-nodist.patch
Source: upstream

Size: 761B

SHA-512 Sum: 73f9698a7edeb9bcb2a15a0f874f71e12396b4751e0bbb8899cba7b6db399a0e7
3b14dc1db8333b6ca49b8053f7052439f04baaaf9b8b83519a96f657a9cff45

### 3.3.3.1. 0022-tests-use-skip_-consistently.patch
Source: upstream

Size: 1.5K

SHA-512 Sum: 039c05919fcde3197a59bf9f512ad6889e55381b8404a8d8c1938ea07963790fd
a44a8ba3d1d007ae67c29507dadb7269394b7b3dcc50535992246a5806c2523

### 3.3.3.1. 0023-tests-use-find-rm-not-perl-to-remove-temporary-direc.patch
Source: upstream

Size: 2.1K

SHA-512 Sum: a8a05a76c2cec0d68bee15c664ef4f1d0db6968f5dda391bd2e9360e98c702a0a
cace813da08f337fca5500330f0f7885bccd88db8f0449a03318c60443d0246

### 3.3.3.1. 0024-lint-make-syntax-check-same-as-maintainer-check.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: 6291f56fc37fd1bd806b6b71e63f9de9c7cea2baca39dab62e9852526e0adbe8f
432156ae7efb889a41ad697b01416a7ad2345fafe4e347aabe86d2db562fdb0

### 3.3.3.1. 0025-doc-clarify-build-tree-location.patch
Source: upstream

Size: 2.0K

SHA-512 Sum: dc3b23f3fd90c154c49d184217277c8edd49e8351f06ef20acd62cf1e38416776
f0ffa7410df096b46edd05dd4002528ac512aefcaaae49587b7018a09b04bec

## 3.3.4. bash
### 3.3.4.1. bash50-001
Source: upstream

Size: 4.0K

SHA-512 Sum: e3bf036287d3be1f3e91755678c04c9a8e1b4a98e34e181871dfaeb13987dda18
c31a44db3f3829d91a185ba4414b9c0229f2a15f6e8a951cbc6c1054252bfdd

### 3.3.4.1. bash50-002
Source: upstream

Size: 4.2K

SHA-512 Sum: 59b1cfa1be1029ada53c63fe651d51451ead5523c50c115e0eada07e34e641c69
3ed728366986acb431f96fdc61818efd3f8cd168ce416001edc62602e5f28dd

### 3.3.4.1. bash50-003
Source: upstream

Size: 6.2K

SHA-512 Sum: 520b5cc0b7aeea6cd8b7471b553d8979996f3627a3e5c8889023562dadc82475b
e243aca2ec608217b78400a1dceb134b877d3ded926e581445234f1b69409e6

### 3.3.4.1. bash50-004
Source: upstream

Size: 1.6K

SHA-512 Sum: cbf51bb242edf36289bd483b47c9451132c12f341f494212c0e5d969cd06a3c1c
4d121295f3bacb1d7d5e56f789258ba9f54c4cfb5760ed3c70ec1f49f25c719

### 3.3.4.1. bash50-005
Source: upstream

Size: 3.6K

SHA-512 Sum: 4d3e6f337a76b9ff1887c4c6e4e4352885779504f3c975b8d6fa587962f01e8ad
bd843b5341c1fc1d11152cf465f2982eebd9dc6e1384f319157d29740d510da

### 3.3.4.1. bash50-006
Source: upstream

Size: 1.2K

SHA-512 Sum: 71df829a3a3927a363ad961de8af8db898ea8b0ccf604c5f1326fe4646d0d50b3
c7038ee473c225fc10d26c2dc1f711d66b74d003bb0445d36a8a70c49e056e0

### 3.3.4.1. bash50-007
Source: upstream

Size: 1.6K

SHA-512 Sum: 467d377836c53d188cda39de550ce1e00b58895a6646c4da3535e74e599978558
a92d8e7bf7c59c988159468fbce04f3a0dbf62cbded28472272f1b9811786e8

### 3.3.4.1. bash50-008
Source: upstream

Size: 2.5K

SHA-512 Sum: 110fef44c1a26819ad8926ce00bd5378e99275763db4b0e9cfd125ba1ab7eb9f9
3abf912efb9841fa2ac59c380995e477683afc8cf6bf00367a9af7ae371e7f4

### 3.3.4.1. bash50-009
Source: upstream

Size: 1.0K

SHA-512 Sum: 6b770dbd4ca1175f9b958931b1e725d96626a24fb270bac5414d1679dde05276c
87654815e9957d6932c515e8792caf8a5f0e9f2dc108bdd041d8024cf75a833

### 3.3.4.1. bash50-010
Source: upstream

Size: 6.2K

SHA-512 Sum: 8ca2cea0264bc0401414207fd8752d4d6eda64be3bb10fdc22529fa2bcedb84e6
ab257ba2badc7078ece7f2ae1e2964635926f227eea7aed58166e82871322c2

### 3.3.4.1. bash50-011
Source: upstream

Size: 1.8K

SHA-512 Sum: 05833d6c85f3795a9c100246335f39155c1b5d190e073bf382269c2bbceb13a2d
e3f85dbe1dd5d4c7824fcca481febe3bdbb4c555e1f2de86bec05fcf6f5871e

## 3.3.5. dash
### 3.3.5.1. 0001-exec-Return-126-on-most-errors-in-shellexec.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 0357bab73726879eb7186ebb2ee07938473ba848411b5a9313890d9ef89a5a153
d53813695936c191e387c78c0af7bb3482d457d65bbca1fddebf5349f7c5962

### 3.3.5.1. 0002-main-Only-set-savestatus-in-exitcmd.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: a5b2214290cbc71b24351718050ba40152b0602af26462f15a545a7369bcb3fa9
35b9e31eabfd5b7112f12909691caf0b7378adead0810bb8f2a17a7ef287aca

### 3.3.5.1. 0003-mkinit-Split-reset-into-exitreset-and-reset.patch
Source: upstream

Size: 2.9K

SHA-512 Sum: b52824a9eba070eae111498995fb1e3bbdd1a21da9029471e53d05f9fbf7e2433
1aebca6b191a564985ac170f779fb61eb3df99b9b113b3f707f9745ed599916

### 3.3.5.1. 0004-jobs-Only-clear-gotsigchld-when-waiting-for-everythi.patch
Source: upstream

Size: 6.6K

SHA-512 Sum: e1ecc8f45f055c744570d9369b7b73583b122d576e1ffb068df5c51195ff9e4ec
4667967bc9cb4fff31862ad3c4d11e535a97ce1a9bc85eba4757f1729228ca7

### 3.3.5.1. 0005-parser-Save-restore-here-documents-in-command-substi.patch
Source: upstream

Size: 1.8K

SHA-512 Sum: ee8411c1b694309af59f23ea518e3a110a2b40c5d3d9359dd478d78b04a6c73b9
3e45996b223d46f2095cd001a43c7828f1a072aaf37efcd1cb1b129359020ca

### 3.3.5.1. 0006-var-Set-IFS-to-fixed-value-at-start-time.patch
Source: upstream

Size: 2.3K

SHA-512 Sum: 9c10829dd038c8a1bbb0bfc91f62b1c3d568a49d5348b190bba7d723c22618628
4d6f969726fbd073c79285c7638bf16b6192393f7c7e1c3d05df5cf8697451c

### 3.3.5.1. 0007-output-Fix-fmtstr-return-value.patch
Source: upstream

Size: 798B

SHA-512 Sum: 260b319a5701cdc2909c845828b618614af57192bd1cd23572cb8e4f74ea1ab97
2304cbae1ec5adc52ead8359d3f3b4e4cbaac99c03dc6c72cf8e53ea9f44975

### 3.3.5.1. 0008-jobs-Replace-some-uses-of-fmtstr-with-stpcpy-stpncpy.patch
Source: upstream

Size: 1.5K

SHA-512 Sum: ba8fe30d47b5e0da90ef25b330659b41f274d0b9823e2a71d74838436d317e2a2
ab6235db78bd81b37f46cf8e44c2f84251a2ff302a54a1d7edb3b889e569d49

### 3.3.5.1. 0009-memalloc-Add-growstackto-helper.patch
Source: upstream

Size: 2.5K

SHA-512 Sum: 89277dc050d17ae9a55a3958c8955b5991669e446832d920dd43ae97caa63b864
2ad034cd95f9df0644a07d731c97e4cfc6abd9b48dc523406f5c196715448a3

### 3.3.5.1. 0010-exec-Do-not-allocate-stack-string-in-padvance.patch
Source: upstream

Size: 5.6K

SHA-512 Sum: b1999f68a303cf8f6222a7157078c382e05338039c72a46afc677b31609d2d370
bc602143434ff9022ab44113bbd49940b95a7b88c6ec11aa5bd89ae93d0883d

### 3.3.5.1. 0011-builtin-Mark-more-regular-built-ins.patch
Source: upstream

Size: 1.2K

SHA-512 Sum: 943423095b2523f67d883c53c748e8afb8e3317406a90ac33104ce4dbfbd2c6d3
2095902dc0313e91eef8e42b72e39362a236b81e19c01c6c975e6a54fbe2014

### 3.3.5.1. 0012-exec-Stricter-pathopt-parsing.patch
Source: upstream

Size: 8.5K

SHA-512 Sum: d8b209254bcece0243ed35e2c00e0ed32a65cd358caaa768e6378ad49685c03fa
91a93c370dd2cc670a881deca65134a7ef29ec9a6f46e5b5c4915a450f377ff

### 3.3.5.1. 0013-exec-Never-rehash-regular-built-ins.patch
Source: upstream

Size: 1.7K

SHA-512 Sum: a73856326f1f5a9bb7c90046ea3d9d782f7e2d2d92b5731fbb7f8f6c069bd8b37
9ebeb4a729379eb70bf48cba6fc49fefe4f2905af6da3e7a3dc956d7e5f84cf

### 3.3.5.1. 0014-eval-Add-assignment-built-in-support-again.patch
Source: upstream

Size: 9.0K

SHA-512 Sum: fe1d650e7dbb25d30ea021dc47322dcfa0d6646369216171ed82fa51d98701390
b95b548749bbac1a0b4f30801e891f159de405d0b4d9d5223220a33320055a0

### 3.3.5.1. 0015-eval-Fail-immediately-with-redirections-errors-for-s.patch
Source: upstream

Size: 1.8K

SHA-512 Sum: f1339a08c4cbf2ad40e9193854f8a7de530ad5f86a50613fd07f08bfdc4acd686
a0e73759b35d151edb4451e20291d0f590cc458474a47d16557749a16b0dbde

### 3.3.5.1. 0016-eval-Replace-with-listsetvar-with-mklocal-setvareq.patch
Source: upstream

Size: 6.1K

SHA-512 Sum: f88ed5a18c803f093c3b8f9488f0dd1d9325cbb05012a37cc5450d785c33acc3d
0ea72a78b1def31a2878a5b2716935320bded405642bf1277e856b141d70a3b

### 3.3.5.1. 0017-eval-Add-vfork-support.patch
Source: upstream

Size: 7.4K

SHA-512 Sum: 1ee90eb7c54fd42c206f02ba4fbe6bd2ac0091d9470ba2f697c060251181b76da
00b61467de390a8ceb4dc4ab02e5f6b663ae05c2d80aca35eea727691f43f79

### 3.3.5.1. 0018-builtin-Use-test_access-from-NetBSD-when-faccessat-i.patch
Source: upstream

Size: 10K

SHA-512 Sum: 2d24b96cba426b8ecb0332170270c0965482cd8fb33bf73cf9b719dbcc6fbaeae
055a634a586ee0167923917df952fb9377f48d724071ecb6ed27af80105df8f

### 3.3.5.1. 0019-shell-Don-t-include-config.h-for-native-helpers.patch
Source: upstream

Size: 1.8K

SHA-512 Sum: 25ec881e857c9c729ad957dee72f4072054961dff7ab51495830ece23ef447993
b92114b07bf69cb0f8fe60e0cdc70317b370e40ac1ff94da64497f35212418f

### 3.3.5.1. 0020-expand-Use-HOME-in-tilde-expansion-when-it-is-empty.patch
Source: upstream

Size: 823B

SHA-512 Sum: 3efd5c25bea2454ebcb288fec7eda64a0b35d6c5c8778a087b242c3f61e8ccdee
56aa3320a4a7c5e67193bdff77e57938ab8039c73e71b7f838be2c1ca3bfd7f

### 3.3.5.1. 0021-expand-Merge-syntax-quotes-in-memtodest-with-flags.patch
Source: upstream

Size: 5.0K

SHA-512 Sum: 4266e0470c108aef46c1f52ee6fb13a815a32aa0aa2472687c49c22cf0c14d8e0
b7ee8c15ce08bb26ade3bef9edc05e7397a1683cebe2ece35545131ab3308cf

### 3.3.5.1. 0022-expand-Fix-skipping-of-command-substitution-when-tri.patch
Source: upstream

Size: 877B

SHA-512 Sum: 5b5793bac1a09ccc76346d7ad35cb6a311f0758a28344b77f29ba21f021a9efda
8dc134917e27786fd9838c7b47bef68b6117c939324c59beb573895fed1e896

### 3.3.5.1. 0023-expand-Do-not-reprocess-data-when-expanding-words.patch
Source: upstream

Size: 14K

SHA-512 Sum: 075bc686a26e7fc754414c49c82eaca4542531b6590ecf79eae23a714a0639dc5
21158775eb927925a730877dc528f7513cbe6f83e8d1feaeb58b056a1e0d0e8

### 3.3.5.1. 0024-eval-Always-set-localvar_stop.patch
Source: upstream

Size: 2.6K

SHA-512 Sum: 85915945396619008d5f0dc5de7847d5fe303f7afdc30027d2f43d6bedf17d068
1ce68441221d13a0afbdbab8f5a9e722c09577552acb5790ff69cd09a3f1229

### 3.3.5.1. 0025-memalloc-Avoid-looping-in-growstackto.patch
Source: upstream

Size: 1.8K

SHA-512 Sum: ff0a65bc04f9cc8d867ccff91337610f94c7d2e6a1a37231f3ecfc8ed643acaab
8e9b2da87c15108ba3f7e089690f230ce0a60ab961bca25d15c676fa6660048

### 3.3.5.1. 0026-expand-Ensure-result-is-escaped-in-cvtnum.patch
Source: upstream

Size: 3.1K

SHA-512 Sum: 188854d3dd7548c593d95a86160cb875d239247d012e6f419553290e5d1c34625
085374fa6e6819ecefd01dd0be6770e9b25dbbd7db6cf1a03e85022c8732b6d

### 3.3.5.1. 0027-man-Problems-in-dash.1-sh.1-sh.distrib.1.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: ca2c7b52bed9e67cbb3eec12eae6258ebbed6bf435452a60c5775691ab6665f66
3aa8eb525765bb36bff0a009b225bb1afad3136694689db12aaecbfefae7094

### 3.3.5.1. 0029-builtin-Default-to-mktemp-not-tempfile.patch
Source: upstream

Size: 845B

SHA-512 Sum: 6278e3911fe5bccb70c4d1170ada1e0b62d6e7b63f04c29e1dfdd790582713660
02b3c5e56ccb11416dbce459cd1aa3123de8bfe608ddccc446cd2ddd085b2c1

### 3.3.5.1. 0030-eval-Report-I-O-error-on-stdout.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: 18acad5e67bee8200671b9402cc1b1b28c5cbdb2845cd3f6899c3fd9a190452c8
a7c4861e86e3a1d4036fe1c3b36809973e18571b9c9bfc053a2ce22fdb830f2

### 3.3.5.1. 0031-main-Print-n-upon-EOF-CTRL-D-when-run-interactively.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: d4301f2bd182065a2c17e88de105ee2f1523591311249bf37de7a7285b4299989
dd54d760131db8c8e21c7f32c57c38739cf59f6dba394011787a20692681085

### 3.3.5.1. 0032-expand-Fix-multiple-issues-with-EXP_DISCARD-in-evalv.patch
Source: upstream

Size: 2.9K

SHA-512 Sum: 7e5bf90dfcf995d779dee8d7863346bf53231c1ce4a30bc2e89bc58c6a82c436c
e20024a402376d8b14f989b420294c04d1474e363fd161bdef054828078d4b5

### 3.3.5.1. 0033-eval-make-traps-work-when-set-e-is-enabled.patch
Source: upstream

Size: 1.2K

SHA-512 Sum: 925e24869d20f9ae0be9961a63598bd568e021efa5d3071478f4d04e2ab973c9a
e5c769a93342db75d8c21014d187aa2d4d2af9b175cfc0267e562e4fce22cda

### 3.3.5.1. 0034-shell-Update-configure.ac-with-suggestions-from-auto.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: dd0fd6b406ee2edcff57a5704a223b61562c4184c11c795a614e57b35cdde5e4a
1aaa8a38c527a60351c3fa9899fb75ba58bc741d32b5cd3ad6b002a86815909

### 3.3.5.1. 0035-shell-Enable-automake-silent-rules.patch
Source: upstream

Size: 1.8K

SHA-512 Sum: acb12f670eef12fd479dbc59da7f395a79f265e949869521904a79fdb586f7c13
328515557661d61f128112976d6a0f5f2b23fb5f74f33ddde1c8f93473fdb15

### 3.3.5.1. 0036-eval-Silence-compiler-warning-about-missing-parenthe.patch
Source: upstream

Size: 1.4K

SHA-512 Sum: 1663acd9c761ecd10b0661ca598f5a6dcddd27f51255cca73993f8ab0f8b1fd07
906712c7da081d3ad2bfaade8a1d1c6561f3948db0ee4ac45fa4d2545a680d6

### 3.3.5.1. 0037-eval-Use-the-correct-expansion-mode-for-fd-redirecti.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: f649c2dcf7119d0ce98e3356177ad42ba2fc81f1c3d7c5fb64d46322b85595de2
6d2d702d718437ecf47982a9edb010c7ae2b97f5db92f81c80ef6f25bfca127

### 3.3.5.1. 0038-expand-Eat-closing-brace-for-length-parameter-expans.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: 447d40b0468d0d3d2de2b82c497e7508ec33fdcbb0f186b55c75a108104c26785
d1b7f84b18bf0e03b6bf4b3b2ede43c3454aeece28af6c351d82c23b73636a0

### 3.3.5.1. 0039-parser-Do-not-push-token-back-before-parseheredoc.patch
Source: upstream

Size: 1.5K

SHA-512 Sum: b9f165e9c206c899e905a1d12f8d1ae41716b4e909238a98ac7042c676789365d
2e764c9ccb6e0bd61f6e9e6c3139a728e4c9f1c2ae54dc9118dc92785cd3bb8

### 3.3.5.1. 0040-eval-Use-sh_warnx-instead-of-warnx.patch
Source: upstream

Size: 946B

SHA-512 Sum: f9159acb17d07bd7e260a39a689450da8fc59845155a9bef78743bf670903353c
5d9f553ad8aec9bc598317bc0c259f98b9de548ca414d097fde1bee1c751eab

### 3.3.5.1. 0041-system-Disable-glibc-warning-on-sigsetmask.patch
Source: upstream

Size: 1.2K

SHA-512 Sum: 0a6102a1f2e850c4bef54819d76180f7cdca9bb1aed5a0cb76eeb65b90e4372a9
0c58a8e81213f3d094fd35da68274480afc0ef169c24933b04aa39ccc646f29

### 3.3.5.1. 0042-eval-avoid-leaking-memory-associated-with-redirectio.patch
Source: upstream

Size: 3.1K

SHA-512 Sum: f72be9583081db7584d595820ec1bec6a68cdeab3d7f47c8af7917cd89f9b696b
6382e95279e8067ac934f50b596153551e928b39024a5d38d983c2f2e05d426

### 3.3.5.1. 0043-eval-Only-restore-exit-status-on-exit-return.patch
Source: upstream

Size: 3.0K

SHA-512 Sum: bc7dead575197844e2e2af2f6f758911229b0d1e8fb0cc0f002180f3a06c62c14
21018ec30efc51623b78a784fd583fb38431a2fe8d940c5d4abcb999b5fd5d1

### 3.3.5.1. 0044-shell-Fix-clang-warnings-about-string-plus-integer.patch
Source: upstream

Size: 2.3K

SHA-512 Sum: 07cbc2552da425209db288d4018142f424fa93080b87ebc970325ad36f275c060
427bc4390894aca9aaaf68796073d834ab522e5dc3501f60b13edf650b2d3dc

### 3.3.5.1. 0045-output-Fix-clang-warnings-about-GNU-old-style-field-.patch
Source: upstream

Size: 2.3K

SHA-512 Sum: c8a26171771a3192165621f4528da3a41b914cf01216d7ceed9a1fd22933ed721
d214181696ba3de0ce82c8e277ec18f25f7b13816bdfcd39d5bdd5c6a109e71

### 3.3.5.1. 0046-redir-Handle-nested-exec-within-REALLY_CLOSED-redire.patch
Source: upstream

Size: 2.9K

SHA-512 Sum: 9bfdb30e8f5244151ec770e582e7be8528b099386d3cb1b8e1bb3d7578719c21a
b287ef5d95802524a317c6682756526f1e892ddfec447a643a8f3fc20cd9b9b

### 3.3.5.1. 0047-options-Do-not-set-commandname-in-procargs.patch
Source: upstream

Size: 794B

SHA-512 Sum: a58a23ab40dadcebd9e3ee446cdd2acef3edf2ce3730d54fdb2a4f2d08dd10a24
184a03030a8b550c61b4b0b426f849b38969558c6a86d12d809ef30fad54757

### 3.3.5.1. 0048-expand-Fix-double-decrement-in-argstr.patch
Source: upstream

Size: 0.9K

SHA-512 Sum: fed67d869a30edbbfb9ea9868478ad667bd392b4d2e5e3bb7592a5bc92ef581b7
a0c7d71fd1a0fb46421d2fabfa971146182723b09fd02383adb2338ecfa54ac

### 3.3.5.1. 0049-eval-Reset-handler-when-entering-a-subshell.patch
Source: upstream

Size: 2.8K

SHA-512 Sum: 6f0f03a16d4a14311bcc917afd547b32b1da0cbb9ccd4cf7dcae7ba09cf9ff336
472a969274ba79050b27d8a283e3f9f18bbd0f85edd25cef18d5ac29dc753b3

### 3.3.5.1. 0050-parser-Fix-old-style-command-substitution-here-docum.patch
Source: upstream

Size: 3.3K

SHA-512 Sum: b4c89db7a823c509fc694306deb5b416cd5c8327b32c006c06af9577be5cb459c
c8ade74b06df2a009c982a8cffcb622230d0fe3cb5b1b49a05707ef54107bed

### 3.3.5.1. 0051-expand-Fix-trailing-newlines-processing-in-backquote.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: f979bc7b55689845c057eba17e91ee8fce589f02b5ca836e6b02758df7c0d187c
9e0276811fb7ba49f787343937787ad0831a31bea266c83c400708f5e8e280e

### 3.3.5.1. 0052-parser-Only-accept-single-digit-parameter-expansion-.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: 652d173ffd600a91115e9ae8e8e7003208667ef759fb796e98b8a12e6f6e81d19
2a6112a838e1f914d1ffca8c741330fce7bfc8e34618cd5e41600ea090a0de2

### 3.3.5.1. 0053-shell-delete-AC_PROG_YACC.patch
Source: upstream

Size: 661B

SHA-512 Sum: 88deb9fc584adbb72dcbb202db81a346342ca8ed2ccb756fb03b8a09fe12b4f89
ef1d19b9aa0edf09ee2ec8ca960f7bdbf6920b094345c1a001062411e79ef6c

## 3.3.6. elfutils
### 3.3.6.1. musl-fts-obstack-0.178.patch
Source: glaucus

Size: 3.2K

SHA-512 Sum: 395f8b2b347f45da40f5c47b9d00d399532aaf2ec2b3c181120fc7c3659516ddd
60d82dee4721634930a301946f579b2e6888be1e8abd45f04ef15f456356bd0

### 3.3.6.2. fix-aarch64_fregs.patch
Source: void

Size: 492B

SHA-512 Sum: 3882d9e6a831cff922485dc46be6ad699b4170964bc1a941c51006b3a1c21d345
73133507aaee3557cf655390c8839728e624694158dec1063adc5bbcd1886d0

### 3.3.6.2. fix-uninitialized.patch
Source: void

Size: 488B

SHA-512 Sum: f8fd9d1ae58238c7a7b8e602b904343a221bb141cacef32c8d1d27be7301018ba
b925b44f013e4758c5aba3ee5ac37a61f8f7c1cc6076ab3379b5faa9d661dad

### 3.3.6.2. musl-cdefs.patch
Source: void

Size: 631B

SHA-512 Sum: 7525da5347d7b3de706966b78b4986f93a45228b78ec01af3a223132520965c2a
f0945fa81ff2fd09cc5259d6b48c3ef23cb34a13c062c91b41bd53414914468

### 3.3.6.2. musl-fts-obstack.patch
Source: void

Size: 1.5K

SHA-512 Sum: a4f3a1c759faa5be215c33afbae4978a02c5fc0ae9b76e516b794cdfa60f0f5ff
ca53cfe181568ec6d370f8373781ba73d90c58c9c37207f3b99c82d1b0b7fa1

### 3.3.6.2. musl-macros.patch
Source: void

Size: 1.4K

SHA-512 Sum: 7cf1cdfdad50d7cb6a1817b64dd0da5cc0c8cfad775804f0e1f9a6eb13c67d3a5
0b3c83c7e411c4627c3969be4d280758d6080c86e1f3f257d5ec1626202a8b9

### 3.3.6.2. musl-qsort_r.patch
Source: void

Size: 1.9K

SHA-512 Sum: 5c4328b7085ecb96ea986650067c52bb5ef44665e51f5b2d0a10ff5b7138fa6eb
9d30c7c249269bdf7227dbfe654e9f100dc43362a359876f3cff16b9bfc2805

### 3.3.6.2. musl-strerror_r.patch
Source: void

Size: 594B

SHA-512 Sum: ed6597395e577f26aac2e134a3729d69b29ca48ba562364d8f75c27bfdbf62e30
5130ce577a6133c85608d8c810482ac35649eaa62865aaed498a532bd303e2c

### 3.3.6.2. musl-strndupa.patch
Source: void

Size: 662B

SHA-512 Sum: 9b8c6e53b9ae87a311fe2e86dc32f87738a6f8365075c750a29078d15520a7708
cd54eb609f3916b1c80e62bb0ef762b080b4f11c266521c74dd0f4cc3fd952d

## 3.3.7. expat
### 3.3.7.1. 0001-Changes-Fix-spelling-of-September.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 2dbae59c617721615687433dd5231317666a3b534fa061d9b353e9bb4f1232864
ac8fa911c102815673b7dc40ae55415ecf9b0a3ede6192a59580bb1f1128564

### 3.3.7.1. 0002-xmlparse.c-Address-compiler-warninging-with-DEXPAT_C.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: d79cf8da23a76833f68f06e6337a109e100007b1caf34a809fa49418f2ac9d025
9ccc2980d243a78e8dad59609eacc1c5600e029f7d6f65f7db0b3628888da4d

### 3.3.7.1. 0003-xmlparse.c-xmlrole.c-Fix-compiler-warning-unused-par.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: bd8d669c2bbbb34e69d4bef87f1475f126dfcdd2a110a9107507b720c3278167b
2ea76ae0561252bac3e4ebac428afbfbd3af5c73d64218a5a2d6ead1203f3fa

### 3.3.7.1. 0004-runtests.c-Fix-compiler-warning-unused-function-with.patch
Source: upstream

Size: 1.9K

SHA-512 Sum: a6b7cf1444d87628974355efb769ff5a786e58eb8284b7e065535efd85c9ac384
512c74980f64c63ca38a50d294269a30ba0e8e3223cef3b8c8893cda1dd88b0

### 3.3.7.1. 0005-runtests.c-Fix-for-DEXPAT_NS-OFF.patch
Source: upstream

Size: 2.0K

SHA-512 Sum: c9ed96d2c66e273108471bad1f68f750f761ea297fc54c10d4c9141b39a923ac6
546348d76f5974f07e1f6bf02fd3ecef375524ad5d9758633bca0258edc0e00

### 3.3.7.1. 0006-runtests.c-Fix-for-DEXPAT_DTD-OFF.patch
Source: upstream

Size: 15K

SHA-512 Sum: e72afa1e997f617cade29980fe962ecc7187a1231a5cd007c0874df8c374a2085
5f136e3c1983612bbedcc6b5bdfcc3c468d94840932c9cc9f766864978d0045

### 3.3.7.1. 0009-Changes-Document-354.patch
Source: upstream

Size: 891B

SHA-512 Sum: 24f73ea1afaa4ccbd74f66774570a65279182a02d248cffd0340b0c3a4d772107
e9c9d1564b1e3bc78adc127626fe76bf74d8fae1dc620bf2b671b21433e2860

### 3.3.7.1. 0010-xmltok.c-Address-warnings-about-accidental-non-ASCII.patch
Source: upstream

Size: 1.5K

SHA-512 Sum: e25fd82aa6bd31dc42d5d11662725bea905a82697bb019915e30b286428e94c9a
387cf1bfadd56c2759adc08436d6e650538ac2cf15f40d9a3c2746aa7f7882f

### 3.3.7.1. 0011-Declare-rand_s-for-MinGW-32-ourselves.patch
Source: upstream

Size: 1.2K

SHA-512 Sum: 35d672124f24a4d8a41f5b4424fce01838f426e10c8fa7d56ffeeb2ce2d84b1b0
4513ab87aace8a302971a155953358750fe7b687d133141f89c971bcacfb86a

### 3.3.7.1. 0019-codepage.c-Define-functions-codepageMap-and-codepage.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: 59cccbf0c8c3cec80063b6acb165e54f9ff22c6eb5557ad81d9f132f8db057882
d63fa995afccce429fb66546a6fb085cd8b80cf9d0a13ac3504463ed24df8b1

### 3.3.7.1. 0022-Changes-Document-356.patch
Source: upstream

Size: 841B

SHA-512 Sum: 1cd485c044c6752afefe2dcd00594ce332fabeb3a268d8e1a871963359c41834d
cee1ec3d804fabdc3e73b546e2eff3084df213b4f2f8d56f7d579022c5fd86e

### 3.3.7.1. 0023-CMake-Fix-visibility-of-EXPAT_WITH_LIBBSD-and-EXPAT_.patch
Source: upstream

Size: 1.6K

SHA-512 Sum: f81f92ebe28d3f3859ba13fef6d9c8d6f6b63b9a8090570c6cd379c608d5d4848
b1c0ca37da1ea3e42b999ee20da9dea87603ec8fcc3ad4cee82c071aa8572e3

### 3.3.7.1. 0025-CMake-Catch-troublesome-build-combinations-for-DEXPA.patch
Source: upstream

Size: 1.2K

SHA-512 Sum: 74a8ce8115b2d4ce2ea57b51bc00d3655f78f80ddba033a930ce7347e784ac79b
3bd8ac3da29cb198e19ba9e644e5644f80016c95bbd2a28518a0ed71b973935

### 3.3.7.1. 0026-CMake-Catch-troublesome-build-combinations-for-DEXPA.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: f16eb21e10804f904590fa3cb9e614c016895e6eaf5df44ded3aa9f88ac8c91ef
b60ef549dec726f242204b9d400e7e74a0a96fb8dee971e49ee7ad3e5ed70d9

### 3.3.7.1. 0027-CMake-Install-shipped-xmlwf-manpage-in-case-of-DEXPA.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: 731d728198a813d3d367a73b796167e73ae881b4d108ba365c0d51a0b34520f1b
8e62f21ac2e3a7f107ae13167cab1a7d55f9c26069d4b6611e4a56186dda3f4

### 3.3.7.1. 0028-Changes-Document-improvements-to-CMake.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: ee14296f115537f0fc33b275e7908f1c6171d1180940751f4c4675cda30dc7abd
1d081564db0a3f2b64c169e6d03e001501f10c0f090da428cab1e7692b5c1dd

### 3.3.7.1. 0029-xmlparse.c-Limit-declaration-of-rand_s-to-mingwrt-5..patch
Source: upstream

Size: 1.2K

SHA-512 Sum: 93700c4a956179a22caad0b83319260dfba5c5e8a52682e6b6899f9a832069f04
d3dd5ca294d3e1d145a585c42a01890392fd84e55ced38e5afdf62b6709fc2a

### 3.3.7.1. 0031-Changes-Give-credit-for-361-and-362.patch
Source: upstream

Size: 673B

SHA-512 Sum: c0e36418e220dae64d7a716b2e09dfe90b4280335dda4e9f2e8d11047f563e3fb
0c5fa13c23e00b141c0b6b15d6faed04939d09ee3215916d0910048fab1d8ba

### 3.3.7.1. 0032-Changes-Fix-name-order-for-2.2.8.patch
Source: upstream

Size: 772B

SHA-512 Sum: fc28baab40bbd407b7d218c0cfdb1c81fca44d6141872d9dcbfa21f5908391b3f
59a485142268ab16a849b65ed52b2f46d1f4deb685c179e254fd0b32de0b8c1

### 3.3.7.1. 0033-xmlparse.c-Improve-warning-regarding-lack-of-high-qu.patch
Source: upstream

Size: 1.6K

SHA-512 Sum: dd5c6504a440526c244f4c9b80021db213e194186819de000de03ba4a9273a3d4
36522a6787d94a3eaecedb4cde4fe62cebc1ae2e8f5512cc51c5eacc8236164

### 3.3.7.1. 0036-CMake-Enable-oss-fuzz-integration.patch
Source: upstream

Size: 3.8K

SHA-512 Sum: 73184238858cd88662abf41e2d96803eca6c08b7bdece6d50d1bb28898b196512
70102c70661859967b8d3b862764d3754c80942eb78a4c3bab83ea650373a18

### 3.3.7.1. 0038-xmlwf-Improve-output-of-xmlwf-h-by-two-tiny-bits.patch
Source: upstream

Size: 2.4K

SHA-512 Sum: 98e9b12698c848c8a45cb871c30a7b9b6e18239c6e0e1e8506bd5398dca2bf42c
3c46090d6c7881656cf454129afaca1ccd1cefe02080bd8850e98facff8e76b

### 3.3.7.1. 0039-CMake-Fix-warning-due-to-if-statement-with-mismatchi.patch
Source: upstream

Size: 948B

SHA-512 Sum: 09f885afc9fc2f546d72c754c5a98bcbc1f25cebc050d94ff2b47835de6c0e573
14a3226b39bc2f93ce49f62296611e403f0b775445a77dbbac8c6d185d048ee

### 3.3.7.1. 0040-Update-COPYING.patch
Source: upstream

Size: 743B

SHA-512 Sum: 5ccbbbdb67d6d606875df463e23f59be600ac9e241b950138bd9808de8d42631a
6cdd357dc2188f58555f74b257c72428b27d2d83669c046b95404b169cd58b2

### 3.3.7.1. 0041-README.md-Replace-should-by-can-regarding-Windows-bi.patch
Source: upstream

Size: 815B

SHA-512 Sum: eac5b4c949af3de3bb3eb998bc619c1e24600447b9c7445b25f79b0f1b859ea10
0df6fd1f26b57dce42f4492e2d32c627e984d0c1f70f646f4f10905acbf77d6

## 3.3.8. gettext-tiny
### 3.3.8.1. 0001-Revert-libintl.h-don-t-enable-NOP-macros-by-default.patch
Source: sabotage

Size: 1.4K

SHA-512 Sum: 0ed7461ea5d9322a91a244c44822bc9eee271faf8d87bbc10d380ef602bb1404d
2e9b4870e4fdde7d77a83c9663c8f3acad9f890f84cca4d946bc086bc2e9d06

### 3.3.8.1. 0002-autopoint-add-sanity-check-for-configure.ac.patch
Source: sabotage

Size: 880B

SHA-512 Sum: bffb11609e37387068a53d15871b364a58dbfe75b7dbead47bd25c3584552d052
569bb8439468ab14fba6fefd170b908645d8a5b7837fa469fd2acb8bbb4de0b

### 3.3.8.1. 0003-Revert-msgfmt-remove-unused-error-function.patch
Source: sabotage

Size: 828B

SHA-512 Sum: 6ebfb37a68366c5569982b8a1ee7a797f305a8e41a6631c0db21edeb4005efc81
d1deb42475f9ae16af450a3f8e9131ef51fd620c9befc1f7c4b964b18f2d44e

### 3.3.8.1. 0004-stringescape-correct-break-condition-of-unescape.patch
Source: sabotage

Size: 1.5K

SHA-512 Sum: 2e1474d6239d6d6937afbf828e9e2fbe1d03773aee86fb4af3d22874eacf95068
83b606b179bc28b7774ac1eb84810d45a750bd1f0958a563d14690d2e78611a

### 3.3.8.1. 0005-complete-rewrite-of-poparser-msgmerge-msgfmt-ported.patch
Source: sabotage

Size: 42K

SHA-512 Sum: 10d69b37a814c52bde833b0c7b6f7a7910a7a2f6111f673e96fdbeb705885b5ce
5722abcd99ac4a0a1fd0c1d0ef107f0d9d7e3a2d89ee63aff3fe2316591f1eb

### 3.3.8.1. 0006-msgmerge-use-the-same-size-as-msgfmt.patch
Source: sabotage

Size: 838B

SHA-512 Sum: 809045196c24684fb6b5f9eae382ab5c38970e56bf2eaf9549f3404f2b1d14cf0
a60bffc87fabcbd76054065052f06de345b3a0b5b05d4c4a95a8000bb425d18

### 3.3.8.1. 0007-stringescape-add-missing-escape-chars-to-escape.patch
Source: sabotage

Size: 1.4K

SHA-512 Sum: dfcd2b7c937efc2348a82a009127150e656140c95736a80ec9d54f4883e7c8cc1
3e58a44b44a040fe2be2b9674f1de78f2833e38af36b024fb2e06b7403b49e7

### 3.3.8.1. 0008-msgmerge-give-enough-space-for-escape.patch
Source: sabotage

Size: 1.0K

SHA-512 Sum: 2837bed1f8cb0d7295c2e88786833ecf8f94c2ea1e09913193e2c0781e2e6a182
d65d3e5704d4a88a9e40e5750221e99e7218d27aa83307ed2342373dbffc24e

### 3.3.8.1. 0009-poparser-not-to-skip-sysdeps-other-than-PRIu32.patch
Source: sabotage

Size: 1.6K

SHA-512 Sum: f010ab8b37150e5eff8c1181729482b99af92329006bf518b9a412da841ddd71e
0e7f838018a37fc72b02a1125db3ba4b37006914221f6f67b96df2c50734d0a

### 3.3.8.1. 0010-msgmerge-pretty-the-output-with-breaklines.patch
Source: sabotage

Size: 811B

SHA-512 Sum: 0320729c3180855f6db7d7083ed4f5a98edf3ddf2d43326ced7b6d8a62f9e5969
8bec3a6c25d0e69d45cb45ae4b3ea5c16145a895974f3dfe1003ebf4b8c41e4

### 3.3.8.1. 0011-poparser-avoid-invalid-memory-access.patch
Source: sabotage

Size: 837B

SHA-512 Sum: 715aaef2585c86fe1a128bf827fd0f7c1e67fbd8bf3ce596d4367db0e84b41b00
b126b685fad555990a2f6136a9ccd70c11c8a463fab2c76957fdde06e445260

### 3.3.8.1. 0012-poparser-optimize-by-saving-strlen-results.patch
Source: sabotage

Size: 1.3K

SHA-512 Sum: b549ea378f093289ecde0c86ee15c5b94bf31b0619cdc26167de198c3c03bb73a
c83ec402b704185699306ccafd2200a13ad1d8069204fde6b32da4af00c837a

### 3.3.8.1. 0013-poparpser-avoid-endless-loop.patch
Source: sabotage

Size: 1.2K

SHA-512 Sum: 611f3b8ca3a701d6eff90ed35e9a2eded845bfe340b7d4d3fa865378ac19afa52
50dde341cb77254468b52c8f095b246942aed8a477f90fe4b2841524c34aa74

### 3.3.8.1. 0014-msgfmt-skip-impossible-cases.patch
Source: sabotage

Size: 717B

SHA-512 Sum: 7268ed0c8a035823cfb2dd24658c46817ab1353a1990b4a396b5ff26fa41f003a
1111747816e82667fb22d4bb25c8e35a1f96ab541ba009c9e4888c9cf906949

### 3.3.8.1. 0015-poparser-a-more-easy-to-understand-sysdep.patch
Source: sabotage

Size: 7.0K

SHA-512 Sum: 27852a1f44802e9189c34e8eb7d291263b4352a77465405bf5b527f444b93ae8e
0c846c35748df5282f19be53038c13fc34120d220a193c8322e3cd3ede561e9

### 3.3.8.1. 0016-poparser-simplified-sysdep-more.patch
Source: sabotage

Size: 3.9K

SHA-512 Sum: 4742d4f214a25bade34710fd8b28b8648b65c97bef9d936c350e3fef532ed646b
10772d348a0accff7b733aac813ad97c07cfb00f399bd521b57e1056b5a86ad

### 3.3.8.1. 0017-msgfmt-add-missing-operator.patch
Source: sabotage

Size: 631B

SHA-512 Sum: daa4a9be3b877b7d0b43ea79bab86d41751dd11e71730d1494d6c00011fb0e4dc
d45c5bcdc52c920630437dd183ab881e6b6a7b91dfddf870a8aeb3d6a79215b

### 3.3.8.1. 0018-msgfmt-add-missing-messages-count-variable.patch
Source: sabotage

Size: 550B

SHA-512 Sum: f857610b61471a424e8f18751406901e9673d04f23d1b148c07ec0ed41eab9e2e
eae9b723d71d45ab09e8f305f601a1bb79472a9de502e69cfff1c1e0f3f2357

### 3.3.8.1. 0019-msgfmt-poparser-correct-length-at-str-table.patch
Source: sabotage

Size: 2.1K

SHA-512 Sum: d3c87e65805e359d6a8fd831c79f9e5358ee02a0c51fa4dc9e40a56d223636832
6e1d1acc55e9b7c06fea8e91c4630f50f22c72d6f848964d792c0064f0f8d12

### 3.3.8.1. 0020-poparser-avoid-invalid-memory-access.patch
Source: sabotage

Size: 1.1K

SHA-512 Sum: ef894d0712bdd757b31b45821181c01a33b6b9484232421a01877981b06a92e23
d844bb516ebb63bace70b125606a7f3d533bb5ea1c9048fe9b99e33a15e4403

### 3.3.8.1. 0021-poparser-avoid-memory-corruption-by-terminator.patch
Source: sabotage

Size: 842B

SHA-512 Sum: 6c947020b70fb887c13d50193d8f4cc2d95f5c0f69a887ecc341e2e94e162d6e7
031d6c640b11aca091c550848ea6d391750f7d8f8e7807d2204330bb58cf4bf

### 3.3.8.1. 0022-poparser-avoid-comparisons-of-different-signs.patch
Source: sabotage

Size: 1.4K

SHA-512 Sum: 1bdbbd55a686fe1bc5594c2f0e395f5e9d0727e52607ae58e550842d11229516e
a71c4403dfe7733c933b233ebb12506c01b79a2386a59f8befb9a024f2ff10f

### 3.3.8.1. 0023-poparser-return-if-the-buf-is-too-small.patch
Source: sabotage

Size: 1.0K

SHA-512 Sum: 5a12573638bbddcaf0d86af2c1e6790ed983d81bdde7feba925dbfe008dddf7cc
242023f39cd93b1f4401356560d488bb88e314ac6cb066a1f2b9be5a9930e2a

### 3.3.8.1. 0024-poparser-set-correct-length-after-parsing-codecs.patch
Source: sabotage

Size: 1.3K

SHA-512 Sum: 2e40a99f81bbb2449a62ba688a0f6a82d21c41720d2eeedf95cfce84e50b89e84
16d21ca994f28360bd48a9263c152b8f66f50d378b967b77f34cc72bfea1505

### 3.3.8.1. 0025-poparser-convert-codecs-at-both-two-stages.patch
Source: sabotage

Size: 1.0K

SHA-512 Sum: 749ec86c5a054494f3d4d7c349914c027ee59da6b579c6fa9248728ae07e2fe8d
d161451e0b077866773e8b32086e87a0fae06e82517d4447ff406c540097522

### 3.3.8.1. 0026-poparser-avoid-32-bit-truncation-by-unsigned.patch
Source: sabotage

Size: 1.1K

SHA-512 Sum: cdbd04fd20ac9a5ae995ffb8f76a8ed08efe07710a8e1da641c9192bbae34398a
27b6319f1f139fc58464b6a3c02d0401d512b112ad132be351f68a9e0bea13d

### 3.3.8.1. 0027-msgfmt-do-not-return-the-result-of-remove.patch
Source: sabotage

Size: 785B

SHA-512 Sum: 7a2f31228079373ecb05bf16a2df9c1150117be998cf527d6e77ab2529f65f7a4
95c663901c1e5e19ce2a157e453e574313eebb38c75508275ff3c8849bd8de6

### 3.3.8.1. 0028-poparser-enable-first-flag-at-both-two-stages.patch
Source: sabotage

Size: 735B

SHA-512 Sum: e1f929f7c8cb76ea00a3668c3235b7d72aa4201e3a92b7de821d3e6966d10db87
d0557c9fba78d1926e1e9b2b078a50d0f4efab24c7d024e2e05eb8a2d279a68

### 3.3.8.1. 0029-poparser-disable-first-flag-after-a-msgblock.patch
Source: sabotage

Size: 1.3K

SHA-512 Sum: 39fffa0b9bcf2044bbf9ad3e7a27eae8f82a840f87dd544305674e3e83b157ea8
f638f202a2d30a554fd1e7dce843c7a915e733f165fce6adf77279fbeebefd8

### 3.3.8.1. 0030-poparser-should-check-length-instead-of-pointer.patch
Source: sabotage

Size: 859B

SHA-512 Sum: 4644847ecc894c009de385c70a1e469503a274e3afcd6fc552fd7ace7dff0e1d1
2ea4797beba003cfc6808f19c1d419a03a8737fea0b7818c486cd4efb1ae949

### 3.3.8.1. 0031-poparser-clean-msg-comment-flags.patch
Source: sabotage

Size: 649B

SHA-512 Sum: 01d4bf244ca4f8b8c0103fe75da11c13669aad264ccd6dd171804a7d0c32a6745
be6da38af125e9cca863e9aa2d85fa0553205d90702f6efb14d9d99ed3676e3

### 3.3.8.1. 0032-poparser-comment-may-start-a-new-block-too.patch
Source: sabotage

Size: 989B

SHA-512 Sum: b2c58717690c26a84229bf25a65ca35b35c66efb8d4955c7fd4eaaba6a4645c1e
8cd2a127555e93c5810b303327b7f39d6d1945d9301f9d76ba257f4c56b560d

### 3.3.8.1. 0033-poparser-add-po_error_last-to-po_error-type.patch
Source: sabotage

Size: 1.1K

SHA-512 Sum: b7d57cf5405b91ac7a8b3cddbe34442da82a096ac7a18c738644a4ae2166c8e39
f0580098875708711f0da0b12e6d2a2ffc66df93738e97e37dc0737712b184e

### 3.3.8.1. 0034-poparser-convert-codecs-at-both-two-stages.patch
Source: sabotage

Size: 2.5K

SHA-512 Sum: fcda707d763d1fca2cb78b38e987fab31926c22876475d9c1342a1019605fa7e5
5175323b920a51dabcc83c4760a1f7ecae542b1014b657a77d83f00a0616ee2

### 3.3.8.1. 0035-poparser-charset-str-should-stop-at-escape-chars.patch
Source: sabotage

Size: 1.0K

SHA-512 Sum: 8b6679463ae6bae7f6fdeea052fb406d2b192d038ce37413405f91e8ac94e610e
f7fc3bc6e084ddff17457d91e2ef9d47cbdd429305963fbea1ea85ee0a22ae9

### 3.3.8.1. 0036-poparser-default-to-non-strict-mode.patch
Source: sabotage

Size: 1.4K

SHA-512 Sum: 36b5d21d5eaf3d9234cfb08ee79f867ce3ccc59361f3f83d0b277bdc2d97af4a8
a2109c2a8ce3e3090766d819b26103379844ee4bdcc4884c5a69c4225579a08

### 3.3.8.1. 0037-msgfmt-enable-strict-mode-with-c-argument.patch
Source: sabotage

Size: 3.0K

SHA-512 Sum: 5c2f69cd8f8ec2ca43bea1132892687e0223d5c109ec517405b664d73aa39a533
f0854d3b67288c4c7c88dc63bacb1b7861c7015636da4dd140574ca6175a572

### 3.3.8.1. 0038-poparser-msgid_plural-is-with-nplurals-2.patch
Source: sabotage

Size: 750B

SHA-512 Sum: 20f8d3237b8f51b3fea2d3fb8eff2cc015a7c852c74f460569ab4f176edf805b6
5443d2dc39e30dd8eb611f7c62e47ef1512d85eb3722dc127030b9b1957bc1c

### 3.3.8.1. 0039-poparser-not-check-overflow-for-msgid_plural.patch
Source: sabotage

Size: 821B

SHA-512 Sum: d162ba5bed2b6c861b36d3057c5ea11dc606221aa630cf3bf113c756325493f9a
0ea278ce66d8ca09ecbf50e68b972a41ee7638c7a4dcfede105fadde68d7b97

### 3.3.8.1. 0040-msgfmt-clean-code-prepare-to-handle-other-modes.patch
Source: sabotage

Size: 5.5K

SHA-512 Sum: 1337068e7a83f9ac420a68b8e8fa79884269d0eda80194d84d7cc145fd2d9aa41
43d166ca1d8c85b46d69a76822c8a90aac292926aed730e55fa98fdd8ed1fdd

### 3.3.8.1. 0041-msgfmt-missing-break.patch
Source: sabotage

Size: 619B

SHA-512 Sum: 9395e64caaf3a72320c140db3e1486a3bbdf14004eceba391176574a3e4adf3d4
52a4d9c83040f0c5a3e810cfc53a3a06558a8f92d4ef7f19bd3dff5d637049c

### 3.3.8.1. 0042-xgettext-parse-arguments-correctly.patch
Source: sabotage

Size: 974B

SHA-512 Sum: a9bd7d973f0b0867df242d99657b06071c4737bc43c6625ff7e7746c4a6f86bc7
a7258f0dd44eada8faad7cee67e603eec9be27778cccaca17a9eababe0b797f

### 3.3.8.1. 0043-gettext-tiny-Fix-format-not-a-string-literal-error-4.patch
Source: sabotage

Size: 2.1K

SHA-512 Sum: f50c3e874dda2369aab05f0886501d8741b7a59e7dc63fd9f0a1a23d0c7ade21a
a765eb249073d1cefd3535335ed24000dcee29e1f44885b718d7b34f3977472

### 3.3.8.1. 0044-autopoint-support-dist-target-to-release-tarballs.patch
Source: sabotage

Size: 1.9K

SHA-512 Sum: a60dd1492b96be8a9c2c4c63a89527ef3b5cbcb875ff5b604a167cdb8bc6744a1
0953f645c0ba82b7bd264e945e6c914f5a98ff228de87c2dda6a0d408d744e5

### 3.3.8.1. 0045-data-Makefile.in-add-missing-maintainer-targets.patch
Source: sabotage

Size: 3.5K

SHA-512 Sum: 07e43b182fd3e8b6bfcc7b39fe4cb75b7e916287f4582a126c2bd720042906fb1
baab50f4cd826b865faf77a67a910368b4584b596f906e90bc2602456807b36

### 3.3.8.1. 0046-msgfmt-support-keyword-template-output-options.patch
Source: sabotage

Size: 1.3K

SHA-512 Sum: c33d71ff6b65ca7992264e890aa83a56d7717c3f6755a1c5da53a942c4ea8ea7b
41ec99edc00def3dd00c780857d673bc965a6675ffab6528d28ef917d0aa6ff

### 3.3.8.1. 0047-Makefile-fix-install-failure-if-path-contains-m4-str.patch
Source: sabotage

Size: 1.0K

SHA-512 Sum: d23b45ab09c41ac91609fda3334c57445d5e82f7fe3fdb754c5771acea1815301
1499670778cd46c1dbccb961385a90c9af2991086b7699720ce5b4eed37b309

### 3.3.8.1. 0048-msgmerge-avoid-printing-too-long-line.patch
Source: sabotage

Size: 2.6K

SHA-512 Sum: edfacc03a928cb28e04b77347c87cf86a6e9cc91f3567a92c21c0b066d2c38050
6a187616d239bf376b7766f1d6bea8df24a8690eea9e61ed8b0b1a092718574

## 3.3.9. grub
### 3.3.9.1. 0001-Lower-test-timeout.patch
Source: clear

Size: 674B

SHA-512 Sum: 14d112dd505eac000339b6620cb4650f388428f03e1d842b74148bf33d8435e3f
b45741a3a6c414e2e9167e3e45b41128fd8f42cd7b494a53182ea9151f1c92e

## 3.3.10. intltool
### 3.3.10.1. avoid-process-race.patch
Source: void

Size: 901B

SHA-512 Sum: 5e5125817785355e15d95a59c34ade78e2daf53b4bec8d3b250adef32c03edd40
d72d7011a6b0f97f93b23f01aa6a082c14eeae19a6ce9582b7e57797c6f1a69

### 3.3.10.1. perl522.patch
Source: void

Size: 2.6K

SHA-512 Sum: d9c6afa9c3979beb78c8b7f268657ea13535289cbeb323216831b2d124b6d30e0
99fec4cb4d2c319ff60913358dfa029fc8e10d8cde4c7bbeb3d3e46242ec1ad

## 3.3.11. kbd
### 3.3.11.1. kbd-2.2.0-backspace-1.patch
Source: lfs

Size: 12K

SHA-512 Sum: d1ec0d322036073f436cdc326d9f3798c2f0dfc2e5222d6703dbb479ebd4f87ce
6ea40e28a67a329f4c44c2c5f45a0fc3ee62d5ef2925766bd3358a8835a95c4

## 3.3.12. kmod
### 3.3.12.1. 0001-Link-against-libcrypto-not-all-of-openssl.patch
Source: arch

Size: 2.9K

SHA-512 Sum: c6d7bef860be23b91ef386a0056b4a31eeac2ad79a28ee38600aa8a2f3556ef11
a8a5e7688dcb44230a9cd8a99eb9cc5f5a2cd9d406abd8c670d2d9a635c7b69

### 3.3.12.2. strndupa.patch
Source: void

Size: 359B

SHA-512 Sum: bcd94153b690c2c721ab50052f4d13c9d2bcc4bc04cd340d51aa9e72d5614b484
5235022b854e6827f1727b9621ce22d066a4bb53752d00bb2a09be9733323f5

## 3.3.13. libarchive
### 3.3.13.1. filter-xz-enable-threads.patch
Source: void

Size: 571B

SHA-512 Sum: b98683212e847d2d06c6796b0238a875df438acd7da4872daa0319d6d20294075
b0634d4781ffbef644df243ae6e93a2fb0f7c8be31aa60c3a1cec8e0d8cedb1

## 3.3.14. libtool
### 3.3.14.1. 0010-maint-relax-sc_prohibit_test_dollar-check.patch
Source: upstream

Size: 964B

SHA-512 Sum: b471e1b933dc71615f4dee29dcc65a75af52931b33d71ba2a657b05a13bb60130
15a2352a27a30fd0fb9ad70527b643ff9da0924fac53c2abcd2a531ff521b97

### 3.3.14.1. 0016-gl-tests-new-tests-for-func_quote-family.patch
Source: upstream

Size: 13K

SHA-512 Sum: 351db6aafe830ec9c66428b084c91198621c746f2a8abd3d3d8e83a98dceb1dc5
afd27b78804f016e748b880a9399ca16c01a6f4b30f11d8480ebe530b3fa1a5

### 3.3.14.1. 0017-syntax-check-fix-sed-syntax-errors.patch
Source: upstream

Size: 2.6K

SHA-512 Sum: d1cd16aa3c37c5d703334674b5f1ac4105f5eee5578a35743395b6b23316c4ec7
ae1d7bea9963c1291d038ec68cf701e04580949f82d24365a32104a3c2bd9f8

### 3.3.14.1. 0021-gl-tests-make-the-failure-more-readable.patch
Source: upstream

Size: 825B

SHA-512 Sum: d22847ec799dda87d49b031c7de09510f75ce4dddad1c6dd30de7d02f83474de3
ce6368611487d6615570927ae96bdaaf40ddebe4c48ec92d9de103c0ff03614

### 3.3.14.1. 0032-tests-fix-objdir-hardcoding-check-with-CFLAGS-g3.patch
Source: upstream

Size: 1.6K

SHA-512 Sum: 9678f5dac8794fd1b1efbd28f8be9372a6f7ca4741919bdbac0ffd8e28ec18a76
b461dbdc23b815f7bce5db39af6d14a8d16523aca037608cba0fa2e00e9b871

## 3.3.15. linux
### 3.3.15.1. 0104-pci-pme-wakeups.patch
Source: clear

Size: 784B

SHA-512 Sum: 09bdc432ba59737d3a72cda9819fba14cf5ed3349ac54640bfca43cd39dbcfa3e
7a979d034462bad3c6900fb4a4a2571ecc29e1f30b391fc781bd704c27aff41

### 3.3.15.1. 0105-ksm-wakeups.patch
Source: clear

Size: 1.8K

SHA-512 Sum: 5edf1a114119308b413c8b988fc55d5389f75a215f77817728c4ad8d175eb4b0c
6b61cf211d56361fda556aec17827f1bb63baecec6052bff42ef8615d48eb60

### 3.3.15.1. 0106-intel_idle-tweak-cpuidle-cstates.patch
Source: clear

Size: 7.0K

SHA-512 Sum: 4a8dc949765b382d20bde32e2a7beba7eba475b09f8fccb2a2d1adb5f1ec66a94
947d619b5764109e559c53451968f94a8337d6c2fb5759e02cdafd4fb9f7dbf

### 3.3.15.1. 0108-smpboot-reuse-timer-calibration.patch
Source: clear

Size: 808B

SHA-512 Sum: 9a9d6990dd453c3f3fa7e0614365921602f423582bf5ace086b8842c052641f46
8e2899816f5f018784235e4001ea739e5385f025bb8bbd418400decad204c21

### 3.3.15.1. 0110-Initialize-ata-before-graphics.patch
Source: clear

Size: 1.5K

SHA-512 Sum: 7098c3d86d86de045e13f9fecf103cc4b9b4caf1f48a0cc97ce655385e00f20a4
6396bad0bce342a109aab07f6c2b31858fdff0e3c61f748825068d09fb34fe0

### 3.3.15.1. 0111-give-rdrand-some-credit.patch
Source: clear

Size: 985B

SHA-512 Sum: 712aced83eced04bf7e0296121fa072e780a17a4df690263474cecbef6c766a41
b21cf1be561cc7c2fc30aa46f83c59f08e3525464647a449904ee022572e464

### 3.3.15.1. 0112-ipv4-tcp-allow-the-memory-tuning-for-tcp-to-go-a-lit.patch
Source: clear

Size: 942B

SHA-512 Sum: 59183a81acf7d121abd960fd0fca153c7e1e350c2dd83bfcd717771b23e71d75b
975e687a68e7efeffe9efe55fc7fa23f9f59eb135d4f2ac9797b33df6a84cc2

### 3.3.15.1. 0113-kernel-time-reduce-ntp-wakeups.patch
Source: clear

Size: 767B

SHA-512 Sum: 43d14161f011b4e4cadb6342cd9d6b769829e70257948a081dd6f7e766501be6a
45ef1bb5c8fdfa2586aa4cf57c7ee34dab014f6f01a320af29ec030236c6f85

### 3.3.15.1. 0121-use-lfence-instead-of-rep-and-nop.patch
Source: clear

Size: 838B

SHA-512 Sum: 15475f00ed045693a2ab89add449c1ad77b66253ff827eb8bab8d1969502403b5
bc9a8ee39a585a144d2dfc23ead4fadf65c3137310c5f8143812baa9e79d906

### 3.3.15.1. 0122-do-accept-in-LIFO-order-for-cache-efficiency.patch
Source: clear

Size: 3.7K

SHA-512 Sum: af2b92ecba32a884733bdf1e137bfa8abf187b880e4cf3501d009afa9282a2b1e
740a6004d154cbc5956efc4fd37e3cb69a411f9aa40131bdb115846bb72fd58

### 3.3.15.1. 0124-locking-rwsem-spin-faster.patch
Source: clear

Size: 992B

SHA-512 Sum: 5bf9076ee95e78dc51d2121948babc66a7fa99c8a4cd5cc2f8102fb1dd225fa5f
1f35d12f1cfa6ab7db9d9e951572eabdd6ae228fd3731c028c46d211d25c65f

### 3.3.15.1. 0125-ata-libahci-ignore-staggered-spin-up.patch
Source: clear

Size: 1.4K

SHA-512 Sum: 67acdcafd2b91eed06a532e456b2d9340a02580dfd559c9b4f5708b2e9e4dda32
7ce7fdd66018523d5c7f29e41d7899261480b7ec2e26669e6c9519528aed9d0

### 3.3.15.1. 0130-nvme-workaround.patch
Source: clear

Size: 947B

SHA-512 Sum: de28edb4b6f5e63650a1412804df93bc8574624392fd6eefa68dac606591d20ed
64a2439c768ee5d91762dec24bb95c46e46dca37c4a63cb597559a26758e3b5

### 3.3.15.2. uksm-5.5.patch
Source: dolohow

Size: 175K

SHA-512 Sum: e0378fc34f01163e0f08c7bfffb1e7771ce0e57f1614ae0a28467a714b88ce33d
559f9e45eb330f71d6071c15684379cd308146213b41e5580ff596501666776

### 3.3.15.3. 0001-libarchive-bsdtar-compatibility.patch
Source: glaucus

Size: 801B

SHA-512 Sum: 170430eac7a32f2b19170c585d3b732af7511a7523d89d6801b06ceb11c61f2e8
d7b17051d17c2566c4517cdaf34df21ac6ea63aa146b405aabecf65aad2ce5a

### 3.3.15.4. enable_additional_cpu_optimizations_for_gcc_v9.1+_kernel_v5.5+.patch
Source: graysky2

Size: 25K

SHA-512 Sum: 52b14ef834769d2b4567e756a4485995acd2e3f5b989cbb53f9b113b42ff67b73
6bbcb284b95fe15c9efb846fd12320a26a131e4ce9af50b521114d274b472f1

### 3.3.15.5. 0001-compat-provide-compat_ptr-on-all-architectures.patch
Source: sirlucjan

Size: 7.8K

SHA-512 Sum: 1daedf0ecea0e75f6ee075e860cf6b5822e5d1c76759e3cec1a3a1c61e183b333
def223c4eb303b5e5c7f8841e89690a67c86b87e6d331144aebc32b81c3eb9a

### 3.3.15.5. 0001-consolemap-Fix-a-memory-leaking-bug-in-drivers-tty-v.patch
Source: sirlucjan

Size: 1.2K

SHA-512 Sum: 21f2737288db0d6975b1b20d60bc3dedbc91f5dae22b7e758577324e463524178
b7beb03bbf237957cd8f4c505aa4e0db14a5bb94ac7d6a5558c92caa9607da4

### 3.3.15.5. 0001-net-sched-allow-configuring-cake-qdisc-as-default.patch
Source: sirlucjan

Size: 968B

SHA-512 Sum: 6fd1b77efac22c108cf02ca3937704582658a8e2078b0d8bfd0baf128f6d94a06
98d315c4fbd9065148afb89399ad0fd7d11ce10bd9782c8c6b09c8a89dab473

### 3.3.15.5. 0002-futex-Implement-mechanism-to-wait-on-any-of-several-.patch
Source: sirlucjan

Size: 16K

SHA-512 Sum: 32603d6e6bc7b9627b8a18b1e3807f3a105aaa3af8e984df20a23e3157829c566
a5401fd331be0a7137195bdfaa80b3951903f6d99dfc9c5665489c03e17f52b

### 3.3.15.5. 0002-init-Kconfig-enable-O3-for-all-arches.patch
Source: sirlucjan

Size: 1.0K

SHA-512 Sum: c4e97986dc3eba213b13bca21c2a4045fba877213f5fb72a500d0edba24c81320
33c0ddfea44d1efab7b98557ed6f95ce1afc081b5a9babd7315e6a401170263

### 3.3.15.5. 0003-block-set-rq_affinity-2-for-full-multithreading-I-O-.patch
Source: sirlucjan

Size: 998B

SHA-512 Sum: f3831199023b34cd32b4fc83824e024dbb6aae8f1bee88fb490f2f167820eee46
007eaf0200a85002a3442e554fbda2c553f0e8c6bc2ab46df211b71b14ed01b

### 3.3.15.5. 0003-sched-core-nr_migrate-256-increases-number-of-tasks-.patch
Source: sirlucjan

Size: 1.2K

SHA-512 Sum: 86647099fffe7d7bea6cc7e6f007e05514ad6c8d9724fac08376985945b03ab1e
f74c121c17d15d1bdbb1990b0164418c2b415e57a6342ff9d2c4519b40b3183

### 3.3.15.5. 0004-mm-set-2048-for-address_space-level-file-read-ahead-.patch
Source: sirlucjan

Size: 918B

SHA-512 Sum: 92293760a99320dda40dc44309d7b4cdb0c2bde39d0786ed044ba2b608d32d841
38c20f01298c6c442083ba0f6d867534966801bab5a89ac25026a899618a4d4

### 3.3.15.5. 0005-kbuild-reuse-intermediate-linker-scripts-in-the-fina.patch
Source: sirlucjan

Size: 3.9K

SHA-512 Sum: a31e73898ab125634386c8f4500de21c14459fa14ac0f1c2e341a93017c943e8b
6f2721a505ca7c4e5671bbea8de93705c24003cb830c2600b57ab89ec6755bf

### 3.3.15.5. 0006-futex-Add-Proton-compatibility-code.patch
Source: sirlucjan

Size: 1.6K

SHA-512 Sum: 7ba968c03d8f39f74737b2d60b3942deeeaf51c5b6c1e32b5bd427430e3a8f40b
40ac0201fdce0fafaf01f05c66ec07922590d70adae5583917431bdd2108543

## 3.3.16. lz4
### 3.3.16.1. 0001-Makefile-propagate-CFLAGS.patch
Source: clear

Size: 2.2K

SHA-512 Sum: bb27af7d445f848fe0dca871b9f38803bb3553fcae10184313dc728dc7e0a0b16
2e4d3153edc5d7a71f02309d696a7923b3244b0a6d8db0ef6cbad3bf29d2222

### 3.3.16.1. fix-make-install.patch
Source: clear

Size: 761B

SHA-512 Sum: e1ad4aceb9cfc6a6417f543a961866b380354f5217535f21353e4766a6c5f62ba
23b930b90c7c70813565c5dad90074567b3bc883882e8f1ec312da129022585

## 3.3.17. mandoc
### 3.3.17.1. 0001-path-for-make-4.3.patch
Source: glaucus

Size: 235B

SHA-512 Sum: 60fce07c7f70f13fb7a72809f685e5f23d9767d2ea7504e4adbab5adc3066becc
602002045279cf6c121140810a147337472f946de8fe9db70c221c398dd707a

## 3.3.18. mpc
### 3.3.18.1. 0005-added-mpc_sum-based-on-mpfr_sum.patch
Source: upstream

Size: 3.8K

SHA-512 Sum: 34cf1395d48bb23f485142a7e9b19bfaf8cd92190d82e37b076e1d57180e62ede
d5ff1efd45ba92021e447918caa61d40368f9a3e9274dd791124858b1d4823e

### 3.3.18.1. 0006-check-return-value-of-malloc-is-not-NULL-in-mpc_sum.patch
Source: upstream

Size: 3.8K

SHA-512 Sum: 26f4b29cd85e117829805073d8e6a328f132c132bd17e28922af3e4fdbdd987e8
33e7196fa47ee0abc027af58272f37d7793c904e29119fcec75b52afded3da0

### 3.3.18.1. 0007-mpc_sum-Cosmetic-changes.patch
Source: upstream

Size: 3.3K

SHA-512 Sum: 5f7ecd6c58d070fde130a6914ff74d4cf907b4c8750f4812bbe68b785e372d1e6
5213505235bbd9452a38c29adc17a311b772bad36f19937fa0edda6cdb66eba

### 3.3.18.1. 0008-added-mpc_dot-dot-product.patch
Source: upstream

Size: 9.4K

SHA-512 Sum: 84bd148a08b9fa255508e35e3bc3132b187cee05ffeb180c068411795b601c033
4b7689ccb6f3c1ddc5815de2068715b930228d540dffe1c5ec657c5840dd11e

### 3.3.18.1. 0009-src-dot.c-fixed-bug-mentioned-by-Trevor-Spiteri.patch
Source: upstream

Size: 825B

SHA-512 Sum: d5d497db5cfd376680b849464ef33ba0bb0322485a41a99344e84ad767f44ec6c
f1e3d9b2046c7e96fa4cd77d261d6bc42d4f7e0c1620816cf6614d0bf7ab470

### 3.3.18.1. 0010-src-dot.c-implement-a-suggestion-from-Trevor-Spiteri.patch
Source: upstream

Size: 2.8K

SHA-512 Sum: 36d7d6195396ce29d49b95ac2da25d3616f8f0c306ea1e92bf141d22d3be0667a
67bd77721181361591dc71dec5ccdbfeaca0dc49f28f855a99606902a688521

### 3.3.18.1. 0011-avoid-huge-inefficiency-due-to-MPC_INEX-evaluating-t.patch
Source: upstream

Size: 5.9K

SHA-512 Sum: bb99e8cfc6b3e33a7d25d0b3cceade338db4a62b0bda0a43b56ad0d8a7e1b2f59
25fe1f8ae92d291873d0e3488854b54be2e802a981325d9294eea4f09b44906

### 3.3.18.1. 0012-m4-Disable-Werror-completely.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 42e8c2de4755e208ca052d2b63b3e9c54a86b8c2144130f7eef3ea8145fab6413
bcf2e676e8263d1a64509c25ab6bbce0c4fdcc37c9c03575c5f436879fdaf2d

### 3.3.18.1. 0019-added-assertions-in-tests-tdot.c-which-fail-currentl.patch
Source: upstream

Size: 1.7K

SHA-512 Sum: bd4bcbef3080b7da7c1bef0151e6e3c7e635cbfe9818640f6d1b5cbe300c35a08
6c9756d9479e9d8af5d988935e3056fe500090df9eaf33fef26a721aac6420c

### 3.3.18.1. 0020-fixed-a-bug-in-mpc_dot-thanks-Trevor-Spiteri-for-ide.patch
Source: upstream

Size: 1.7K

SHA-512 Sum: 9afb21b307707a85bc52606cfa398efffec82662439da386abb59114fbc49fb92
b43a480d7406d6b9c6b42a178eddd75182d2c510e407f6dd09a0310cdc4047d

### 3.3.18.1. 0021-improve-mpc_sqrt-avoiding-the-use-of-mpc_abs.patch
Source: upstream

Size: 3.5K

SHA-512 Sum: 9edb37ff17213f128d025ca753ad8fa41fae7a21870645983ffe8983c92559209
451cf3e3ccaf191068893b8d582f784b3e19a039c665fba064f41898ae04d3b

### 3.3.18.1. 0022-added-example-which-triggers-a-bug-in-mpc_div.patch
Source: upstream

Size: 2.0K

SHA-512 Sum: ad8fbbca02c4d36ac9fe2a56c00a6a948204aba72433fcc33b3250ad37a9ed6c2
d5be1f3a305d65349747344ef396007f96cebd6414fb8707e0927db0dc8334e

### 3.3.18.1. 0023-Whitespace-edits.patch
Source: upstream

Size: 2.2K

SHA-512 Sum: b29ddfc4c3685f51a9d3d689c2b1c64b35667138ff6479137d76d3646450e390d
c0327eb63c14190b0f13950b386e9e4e004fe88c599df45331bc122f8af297e

### 3.3.18.1. 0024-improved-mpc_div-using-scaling-of-exponents.patch
Source: upstream

Size: 5.4K

SHA-512 Sum: 0a7e3a1db8be751957b8bd9fa81705a080ed49e1be1388f378362b15ab93e16d6
f16b2233afd1fe83bf0b1133e6df77cec39150e3b22d2a3c53b8ae1739d1487

### 3.3.18.1. 0025-removed-stray-backslashes-in-the-html-version-thanks.patch
Source: upstream

Size: 2.4K

SHA-512 Sum: 08445ca5c0a4f4528d0a84074b3d37dd593806b6b46d7191cbaec6d7391ae0f45
d9867c66cd716343351868142b52939fd048da5a9d77ef7713047a11450b9f6

### 3.3.18.1. 0026-log-log.patch
Source: upstream

Size: 614B

SHA-512 Sum: cb5f3f8e05ca51e9dac6d6a018a06a48866804528beaffca4c9154e9c4e8dc778
44d3e7e29d5d6e2a94f5019bbd92ee09483dc5b012cd4a3ef38a1b871b1759d

### 3.3.18.1. 0027-added-Known-problems-section.patch
Source: upstream

Size: 880B

SHA-512 Sum: 33390a68a7c1188343cf6accdbfbe5608ed64d0e7940ce25d400d1b3820569168
8e53c52482958d2525146be6cfa8be7cacd0cf9910b964bbb773a69480eb2b2

### 3.3.18.1. 0029-added-reference-to-Pascal-Molin-paper-on-erf.patch
Source: upstream

Size: 0.9K

SHA-512 Sum: cfe8440c5fb32e42cea63eb59cee38dca441130313f6fe3584773c805e9edc69c
97924533ea1818d05560cd2c659fcafdcfd1c84db0b6db1dd6404b5e6537a5e

## 3.3.19. mpc
### 3.3.19.1. 0005-added-mpc_sum-based-on-mpfr_sum.patch
Source: upstream

Size: 3.8K

SHA-512 Sum: 34cf1395d48bb23f485142a7e9b19bfaf8cd92190d82e37b076e1d57180e62ede
d5ff1efd45ba92021e447918caa61d40368f9a3e9274dd791124858b1d4823e

### 3.3.19.1. 0006-check-return-value-of-malloc-is-not-NULL-in-mpc_sum.patch
Source: upstream

Size: 3.8K

SHA-512 Sum: 26f4b29cd85e117829805073d8e6a328f132c132bd17e28922af3e4fdbdd987e8
33e7196fa47ee0abc027af58272f37d7793c904e29119fcec75b52afded3da0

### 3.3.19.1. 0007-mpc_sum-Cosmetic-changes.patch
Source: upstream

Size: 3.3K

SHA-512 Sum: 5f7ecd6c58d070fde130a6914ff74d4cf907b4c8750f4812bbe68b785e372d1e6
5213505235bbd9452a38c29adc17a311b772bad36f19937fa0edda6cdb66eba

### 3.3.19.1. 0008-added-mpc_dot-dot-product.patch
Source: upstream

Size: 9.4K

SHA-512 Sum: 84bd148a08b9fa255508e35e3bc3132b187cee05ffeb180c068411795b601c033
4b7689ccb6f3c1ddc5815de2068715b930228d540dffe1c5ec657c5840dd11e

### 3.3.19.1. 0009-src-dot.c-fixed-bug-mentioned-by-Trevor-Spiteri.patch
Source: upstream

Size: 825B

SHA-512 Sum: d5d497db5cfd376680b849464ef33ba0bb0322485a41a99344e84ad767f44ec6c
f1e3d9b2046c7e96fa4cd77d261d6bc42d4f7e0c1620816cf6614d0bf7ab470

### 3.3.19.1. 0010-src-dot.c-implement-a-suggestion-from-Trevor-Spiteri.patch
Source: upstream

Size: 2.8K

SHA-512 Sum: 36d7d6195396ce29d49b95ac2da25d3616f8f0c306ea1e92bf141d22d3be0667a
67bd77721181361591dc71dec5ccdbfeaca0dc49f28f855a99606902a688521

### 3.3.19.1. 0011-avoid-huge-inefficiency-due-to-MPC_INEX-evaluating-t.patch
Source: upstream

Size: 5.9K

SHA-512 Sum: bb99e8cfc6b3e33a7d25d0b3cceade338db4a62b0bda0a43b56ad0d8a7e1b2f59
25fe1f8ae92d291873d0e3488854b54be2e802a981325d9294eea4f09b44906

### 3.3.19.1. 0012-m4-Disable-Werror-completely.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 42e8c2de4755e208ca052d2b63b3e9c54a86b8c2144130f7eef3ea8145fab6413
bcf2e676e8263d1a64509c25ab6bbce0c4fdcc37c9c03575c5f436879fdaf2d

### 3.3.19.1. 0019-added-assertions-in-tests-tdot.c-which-fail-currentl.patch
Source: upstream

Size: 1.7K

SHA-512 Sum: bd4bcbef3080b7da7c1bef0151e6e3c7e635cbfe9818640f6d1b5cbe300c35a08
6c9756d9479e9d8af5d988935e3056fe500090df9eaf33fef26a721aac6420c

### 3.3.19.1. 0020-fixed-a-bug-in-mpc_dot-thanks-Trevor-Spiteri-for-ide.patch
Source: upstream

Size: 1.7K

SHA-512 Sum: 9afb21b307707a85bc52606cfa398efffec82662439da386abb59114fbc49fb92
b43a480d7406d6b9c6b42a178eddd75182d2c510e407f6dd09a0310cdc4047d

### 3.3.19.1. 0021-improve-mpc_sqrt-avoiding-the-use-of-mpc_abs.patch
Source: upstream

Size: 3.5K

SHA-512 Sum: 9edb37ff17213f128d025ca753ad8fa41fae7a21870645983ffe8983c92559209
451cf3e3ccaf191068893b8d582f784b3e19a039c665fba064f41898ae04d3b

### 3.3.19.1. 0022-added-example-which-triggers-a-bug-in-mpc_div.patch
Source: upstream

Size: 2.0K

SHA-512 Sum: ad8fbbca02c4d36ac9fe2a56c00a6a948204aba72433fcc33b3250ad37a9ed6c2
d5be1f3a305d65349747344ef396007f96cebd6414fb8707e0927db0dc8334e

### 3.3.19.1. 0023-Whitespace-edits.patch
Source: upstream

Size: 2.2K

SHA-512 Sum: b29ddfc4c3685f51a9d3d689c2b1c64b35667138ff6479137d76d3646450e390d
c0327eb63c14190b0f13950b386e9e4e004fe88c599df45331bc122f8af297e

### 3.3.19.1. 0024-improved-mpc_div-using-scaling-of-exponents.patch
Source: upstream

Size: 5.4K

SHA-512 Sum: 0a7e3a1db8be751957b8bd9fa81705a080ed49e1be1388f378362b15ab93e16d6
f16b2233afd1fe83bf0b1133e6df77cec39150e3b22d2a3c53b8ae1739d1487

### 3.3.19.1. 0025-removed-stray-backslashes-in-the-html-version-thanks.patch
Source: upstream

Size: 2.4K

SHA-512 Sum: 08445ca5c0a4f4528d0a84074b3d37dd593806b6b46d7191cbaec6d7391ae0f45
d9867c66cd716343351868142b52939fd048da5a9d77ef7713047a11450b9f6

### 3.3.19.1. 0026-log-log.patch
Source: upstream

Size: 614B

SHA-512 Sum: cb5f3f8e05ca51e9dac6d6a018a06a48866804528beaffca4c9154e9c4e8dc778
44d3e7e29d5d6e2a94f5019bbd92ee09483dc5b012cd4a3ef38a1b871b1759d

### 3.3.19.1. 0027-added-Known-problems-section.patch
Source: upstream

Size: 880B

SHA-512 Sum: 33390a68a7c1188343cf6accdbfbe5608ed64d0e7940ce25d400d1b3820569168
8e53c52482958d2525146be6cfa8be7cacd0cf9910b964bbb773a69480eb2b2

### 3.3.19.1. 0029-added-reference-to-Pascal-Molin-paper-on-erf.patch
Source: upstream

Size: 0.9K

SHA-512 Sum: cfe8440c5fb32e42cea63eb59cee38dca441130313f6fe3584773c805e9edc69c
97924533ea1818d05560cd2c659fcafdcfd1c84db0b6db1dd6404b5e6537a5e

## 3.3.20. netbsd-curses
### 3.3.20.1. 0001-mac-compat-don-t-redefine-__dead.patch
Source: sabotage

Size: 609B

SHA-512 Sum: f12ac38d43aee8d3b7e717b4d6ef6160d849c42e980f8485170d45d52bb756e30
7e8bcc0d8f2ce54b1f07d6fa0522cd614d1821a4440e93ea000dcf07df532c1

## 3.3.21. oksh
### 3.3.21.1. 0001-Remove-clear-line-from-example-.profile.patch
Source: ibara

Size: 674B

SHA-512 Sum: e22459995a00fddcc5b0745bbace8c80ecce55ab6b4c2abb0f24013bf1521abf9
e3fc8d8475744eb778cd61ea02ea30429919a6152e784832340f115d5136738

### 3.3.21.1. 0002-Update-to-latest-ksh-code-fixes-a-hard-failure-with-.patch
Source: ibara

Size: 1.8K

SHA-512 Sum: 9f203c9b2dc7a1a09330ca763a9057f0e3332e6a0079b3f97e61d8951b33b35d8
1b92b03be792279785c8e8829c37d718af3d92ab97a19c8bb3ac47a306496e8

### 3.3.21.1. 0003-Manual-page-updates.patch
Source: ibara

Size: 1.1K

SHA-512 Sum: ff47677c3cb3d62e69b120f876d28daa69644bbf6b9ce984f6019f7cf21aa8af3
0eb7ba6f8f58d4d79b25a19ea6f078ea819b738580afcc8ce7a4af57b20f7f3

### 3.3.21.1. 0004-portable.h-midipix-port.patch
Source: ibara

Size: 1.3K

SHA-512 Sum: 8d50e9790ae585e92c9db0662c14bc932624ed5a56c51645d807b60ff76525fbb
721bd9821e9ec61adf9114e82a33352adfd80941114ab66b5eca808b8826167

### 3.3.21.1. 0005-Add-midipix-to-the-list-of-supported-systems.patch
Source: ibara

Size: 551B

SHA-512 Sum: 4e2b0ecd3b96db6ab752a2016dd81e316e6f9a56b214343f3f93175a22d3156f9
1a529fd8bd79b5dec41da94470eccbcf6384a344c3878929726db52c382886d

### 3.3.21.1. 0006-configure-Implement-bindir.patch
Source: ibara

Size: 2.6K

SHA-512 Sum: a7b0f6a532064ec90f81dba5dde98210f94eeaef7ac4721eb9d3c070f7621f02d
530a8349c4ad0769ab31a13a22e93e293de6ca65d5b5a0250210ff6a3a9d006

### 3.3.21.1. 0008-Tighten-configure-a-little.patch
Source: ibara

Size: 1.3K

SHA-512 Sum: 175c77e8c5b1c55887347838ca3169c554f2be371ca208372b3998eec4acd1ec2
2941a4b6d3ba61b073d5f76c2ef4d28c987f2f2bd2067972e83d500138b4698

## 3.3.22. patch
### 3.3.22.1. patch-2.7.6-CVE-2018-1000156-fix1.patch
Source: gentoo

Size: 3.3K

SHA-512 Sum: d4a01bee11d7c68cff9e1f55d6e231d72cb138511779b5f9347f2bc1d035055d8
bc5f93e98a3bd0970659253f27bdd15151c8e9cfee5f2fb51ff148e106dcda5

### 3.3.22.2. 0001-Avoid-set_file_attributes-sign-conversion-warnings.patch
Source: upstream

Size: 813B

SHA-512 Sum: 061e13e2285648b08bb85e7218fdbe74c2619fa9060ceb98b31641e643c25132e
469d4cd41bd2a91a41a144793f671dd35500032774d04c7fdedca6a93d738e5

### 3.3.22.2. 0002-Test-suite-compatibility-fixes.patch
Source: upstream

Size: 3.0K

SHA-512 Sum: 672c3f3adfb2d67d7704cbb1ae8b9b4c40828994f6e20cb13c707534f81a45c86
4a14c270b972a1e6b32c88f5dfdb0220f1414d8403cc0492002392ef5f6649a

### 3.3.22.2. 0003-Test-suite-fix-Korn-shell-incompatibility.patch
Source: upstream

Size: 651B

SHA-512 Sum: fb8ce8f1cb45cbe1a4efee8df75433088d299be12b776085c0e85591a9a52a095
4ff016e66c3aaba7b359b07f0c23389ff7d68c05a424073d6c0399d18811cdf

### 3.3.22.2. 0004-Fix-segfault-with-mangled-rename-patch.patch
Source: upstream

Size: 983B

SHA-512 Sum: 8527326589178842dffa8e0df3bb3dec1e62f2faaf2a0e4b5813eda372cfd52a0
aa013e481f1ed51e3c3d17e189531a38246065d05a95638e79656a19c5ccafb

### 3.3.22.2. 0005-Allow-input-files-to-be-missing-for-ed-style-patches.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: 95d9380fa41969923c2697585a40d8d3a27daefbed1f3abbb9500a29dcba2dad4
57f499f47c5b6ad4acd33722ae94df7c7750720714f1705bc0c38fdc3c6e189

### 3.3.22.2. 0006-Fix-arbitrary-command-execution-in-ed-style-patches-.patch
Source: upstream

Size: 5.6K

SHA-512 Sum: 0750a36b6ed01c7a3f83a8c7d70369f378026ba644ae860ab44c5fd8bad1c09ad
d1494670c75b8bf76aabd08a4a835bfa9c2aaefc23f7adc0c009cf35db56ab8

### 3.3.22.2. 0007-Invoke-ed-directly-instead-of-using-the-shell.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 029b0ca710f3c34279460f7f37db49122db2e5e47d49f460858d25e87448c6b7c
50b3fb96516444cf16a4f96488560139ea15e0c322037a6448fdc3e0573ec7b

### 3.3.22.2. 0011-Fix-check-of-return-value-of-fwrite.patch
Source: upstream

Size: 2.8K

SHA-512 Sum: 6801c3ed7ff6bbb71ca62812e5616fa8276f41f19d6c84024aa431e1d7cf9e3d0
941e0c3d42799bf90c7db3d595ddc269c59547f10d4a680588323df834a9ca9

### 3.3.22.2. 0012-Fix-ed-style-test-failure.patch
Source: upstream

Size: 682B

SHA-512 Sum: 59e01105a3b65f15537d281abce7aedeb81498dd1d9cd7a9260e9104567785333
d216fa13bbcf5ebc73db5d9280076e5cabb232e6221aeb21beb27f175fc0d93

### 3.3.22.2. 0015-Don-t-leak-temporary-file-on-failed-multi-file-ed-st.patch
Source: upstream

Size: 1.8K

SHA-512 Sum: ca750167d69a510877f76abd9861d788e8017de6f9acfb49779288e4ee620ee2e
b866a13974878ba5db94a992922f82402f973c8d0a484153ab1a1e274fc157a

### 3.3.22.2. 0016-Make-the-debug-2-output-more-useful.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: a4b99185278750831ad9ed05ce5838069db8ea437f03fd6262f780f14a94c9413
a05b61b1bfe920e16637603c65ad1294c51f98a4770767f92de4b9f4515e1ea

### 3.3.22.2. 0017-Fix-swapping-fake-lines-in-pch_swap.patch
Source: upstream

Size: 853B

SHA-512 Sum: 9cb329e7da6acd884e130022abc15b8343a855b822f978d147e67389bcc375a1b
430195e4580f49a7dfa0f112752a096599c83eba0232e79ebf1273735cbff7f

### 3.3.22.2. 0018-Improve-support-for-memory-leak-detection.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: 9a57313d3fdd62c3a76f1b38995db9133b782a8a8753b3fcb3d7fbf42607fbe7b
5a4aaf93e0a8f30242f750f90d4bf207a17ac38bebeb024c690fb98e4946146

### 3.3.22.2. 0019-Skip-ed-test-when-the-ed-utility-is-not-installed.patch
Source: upstream

Size: 543B

SHA-512 Sum: f665a51764d0a2bfc2669fb53eabe20c81cd651a80d4f41d8326161539aaf38e6
5a27d0679fcb9af76dfa6799b5fd603470a3ae3daab02ffd280adcc4a8cfbbb

### 3.3.22.2. 0020-Abort-when-cleaning-up-fails.patch
Source: upstream

Size: 1.4K

SHA-512 Sum: 596a93959188f3bde32b01dbfe63322667f782bf3db7d9301d3857c19abe11916
8ca83158881bc11c34153dc8010aff554802c5067c09d334c00a66c085d2b72

### 3.3.22.2. 0021-Don-t-crash-when-RLIMIT_NOFILE-is-set-to-RLIM_INFINI.patch
Source: upstream

Size: 2.9K

SHA-512 Sum: 21cf3ccf8cc06c7f29a3d4f21b5519ac8db089a795bdc55f1ae7158ccda2d6824
a7d3ef0850f616fec08cb3b477575a1c0ebc3a7e474001e96902f4eff9128f7

### 3.3.22.2. 0022-Don-t-follow-symlinks-unless-follow-symlinks-is-give.patch
Source: upstream

Size: 3.6K

SHA-512 Sum: 74f4668e31541c2cf9140385b5bab281c7edd09886af1a8cc30924d3b69243d2d
9e88aea66a213353348e6ba3d375aff87ec82033e66a3610530bb463d789272

### 3.3.22.2. 0023-Avoid-invalid-memory-access-in-context-format-diffs.patch
Source: upstream

Size: 731B

SHA-512 Sum: 86870efc2b0e376d492b77dbe1876826f677ab19d9f80db4f77fdd42f3f71a658
567410bb5d1d7e6f95e5c22a062ea4110c090696b287747e02b2e6318e23f14

### 3.3.22.2. 0024-Fix-failed-assertion-outstate-after_newline.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: d3d5240aa44eabc826bdebe5c2ab5ac0adb153967ff9e7c83a455030a429ab55a
101d2e0b9593859156ad175d7b9261a464b52af18c710da27af83753abd5936

### 3.3.22.2. 0025-Add-missing-section-tests-to-context-format-test-cas.patch
Source: upstream

Size: 2.1K

SHA-512 Sum: f3a72199f3a1f6a619694a63b97868fe0117ac02783e98e8b68f555fb6414ad14
4ce61043c8e1a7050841fa090b63178b3110dca56603179449699516bfed447

## 3.3.23. perl
### 3.3.23.1. 0001-Add-option-for-pgo-profiling-test-with-perlbench.patch
Source: clear

Size: 1.0K

SHA-512 Sum: 87b884e6af4dd5aacbc18a957aa3eca66cbe040662f42a0030ac826628ccb0724
d5dba768a18a5f3b7a73f6f80e49110c39943909a687ecde0cae65670260975

### 3.3.23.1. 0001-Add-perlbench-for-pgo-optimization.patch
Source: clear

Size: 359K

SHA-512 Sum: 8e79cdf6d802ca1e647132103ed583c54573c6b46086b9408ba988ee9a30a1c06
a87d64849e54def61b48f5fb7c957b4fbc6996b3eb48bbe44d3d3e0604a4ce0

## 3.3.24. procps-ng
### 3.3.24.1. use-utmpx.patch
Source: adelie

Size: 3.2K

SHA-512 Sum: 6683b94f64848721ebce8254461fbd70a3efd048bf9579c5bbe298bd1ec00594c
05640327f0e03475e583607f1f7405139b93fc9f06592d5593174cbf6d4119f

## 3.3.25. python
### 3.3.25.1. 0001-Add-pybench-for-pgo-optimization.patch
Source: clear

Size: 221K

SHA-512 Sum: cd19db38c66c4752249c3dc2c364743d1bb1469a39be037cf61a6fc86b543c50f
20c459a1d2aed5f540e406148cf73606b8471ad26c2de2ea074532124495d3d

### 3.3.25.1. 0001-Fix-python-path-for-linux.patch
Source: clear

Size: 588B

SHA-512 Sum: c39bfc949d4023a80512b97633fba76e1906ae54a2f7255458b66042d69e54029
218b140c584ccc77ccac19134ee9c342bdc77cc2f7b8eca39678b2e500d9cc4

### 3.3.25.1. 0001-use-pybench-to-optimize-python.patch
Source: clear

Size: 817B

SHA-512 Sum: 003cdef8e0e85db4bc595654f29b6a9621c074749608b35ed61b387c826ba409a
465a142368d8ea5e51a2c224d8f10f812fb49d91fb1b5dadaa89551240c5c70

## 3.3.26. rsync
### 3.3.26.1. 0001-Prepare-the-repository-for-more-development.patch
Source: upstream

Size: 5.7K

SHA-512 Sum: 6b26bc82cf910a9753768d07c69a657a1235da8dddd6be040f8fd995736131b31
e1e8a0dbd951cfcae58934d512a53f4e4a7dd0be54a2eb4cc975a03d6e6ea05

### 3.3.26.1. 0002-Allow-some-pre-post-xfer-exec-shell-restrictions.patch
Source: upstream

Size: 4.6K

SHA-512 Sum: 179822bcfb600e1321a970c58593f1ef41552f1f17960ebceb225b3ab2b087e99
65dee7c28edb4d42ff14744dfbf93cc5fdb138c2274e4399f79daa374e2183b

### 3.3.26.1. 0003-Avoid-a-compiler-error-warning-about-shifting-a-nega.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: accbc175047d52923f1b688a7999ce95d53368646a11ac9150d77543e36f347e0
bb582bae2d64f0265f037f2d5df26e544711ff4aeb47c3073b88e49755c169a

### 3.3.26.1. 0004-Need-to-mark-xattr-rules-in-get_rule_prefix.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 47a75a883872b7e350a23d30089d379ff9c1e532a63466a3013c73a87ca4e096e
dcdf7a507f8089daefc9b121009df0ad6b7b8b6509414b8dce2aad988581bd0

### 3.3.26.1. 0005-Fix-itemizing-of-wrong-dir-name-on-some-iconv-transf.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 2e89cf51f2c4b3ca41483cda4ad09ee68824dadb535bf183c5d445d2b0a62f6db
ccdee111b6774421f073e0959bf0459c3ea4fd0eef817e66411f707d69e7453

### 3.3.26.1. 0006-Document-how-a-leading-comma-changes-the-gid-parsing.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: 0cc8b71db4d257e2a77e03f9104090b1c6fa3721a20e0681c146252838f148c4f
bd4b417ff99d39abb9b1a09adc2325cc6ee16c08274fa168ac05c85bbc4000a

### 3.3.26.1. 0007-Don-t-force-cygwin-to-solaris-ACLs-anymore.patch
Source: upstream

Size: 750B

SHA-512 Sum: fcf981de47f63114b9eb0d647608e555f5ce8228a8dd39e0e42447506c001172f
f818b777b2899ef0d0e58de0f7266e2081ed7fc5f730011768dcd1992f6476f

### 3.3.26.1. 0008-Try-to-be-clearer-that-append-verify-isn-t-a-general.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: 671ffde7ef5d6a873c6454f91ba3c26cc5a07c54264a5750130ed7ab9cad38daa
1c76f15ce622b4e6bfc27bf47e3d2a28963fef984972396b6c3838d9d9d16b1

### 3.3.26.1. 0009-Avoid-a-potential-out-of-bounds-read-in-daemon-mode-.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: dc7c5e00adbce7a39694feed245554d24faed1d6a005044d9f6a5cf23a7afc3f4
04a0087a6a3fc4868065597bc89853f8ddd1bfbdcbe4b6aa4c4285444f7c52d

### 3.3.26.1. 0010-Silence-fall-through-warnings.patch
Source: upstream

Size: 6.7K

SHA-512 Sum: 6e3a5b8640396ecc7d618a6ec43203c3fd79450495d22079e6d3ec61a137dcab0
0c243c934b591059017b7be82b7dc898b4030f8603e74b1c612e3210c27f334

### 3.3.26.1. 0011-Avoid-a-failed-test-if-dirs-report-1-hlink-e.g.-WSL-.patch
Source: upstream

Size: 0.9K

SHA-512 Sum: e08d518972f0c1ec100f1905d50761a4a93b3b0b4aee8a1078fc730b9033eebbc
4c14397467c753a388f4ef19f4cca69906b8802a99df05ac0fb71bb80399e68

### 3.3.26.1. 0012-Fix-2-spelling-errors-pointed-out-by-bug-13734.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: df59ba9dab41cb8e71c5a5ad43f7accf33f81f8bd942e20b9ad9105a8deea08a2
4fd7072231a67e854dcdc83e3e1413afc152150f9e3c9a49140e2d3167503c0

### 3.3.26.1. 0013-Avoid-a-yodl-macro-warning.patch
Source: upstream

Size: 790B

SHA-512 Sum: a6c395366cc8d1a2795700f7c3cd493afb7714291eec88634ed7a55cd74e380df
e4181ec905668765e75c7db89b9cef7ef1e5724bb37b0f0b333c9de932f7621

### 3.3.26.1. 0014-Make-sure-that-some-memory-zeroing-always-happens.patch
Source: upstream

Size: 1.8K

SHA-512 Sum: dbca90f33f67b0394ac788e8ac8b885264d8f3aa6b9beb41b2c4a9ac438ef9287
b41ddb8a1896b2ee0bc02474a5f4f01ad5bc9b3a6820531a6433829932602bc

### 3.3.26.1. 0015-Avoid-a-yodl-macro-warning.patch
Source: upstream

Size: 1.4K

SHA-512 Sum: 5f9c879fcf0f22d3f1a8e1b098bd37ba66fa57cd4700c601c0be902f702cf4990
4a4b0e613eaf92de64db3090ffdd0e3305a17e8fd2d2976a2cc695049ee8afa

### 3.3.26.1. 0016-No-need-to-strdup-each-new-section-since-we-stopped-.patch
Source: upstream

Size: 2.0K

SHA-512 Sum: edab8b8596ca4bd506f69546da0dbbc798c1ec4a800e525bd1fc39fcd060eb0fb
ed75846b54eca10451dfe3141225823e1404963fb620a5d8f17e1815291d6c2

### 3.3.26.1. 0017-Save-each-expanded-daemon-config-string-on-first-use.patch
Source: upstream

Size: 5.7K

SHA-512 Sum: 943391378006dec15dea8cd3147309ea304267a4d8c25476acecbad22a262ab9e
dec7c2782a5881294f07ff8adbb4554fa86a99592940d1a0bc7c8800fa6e343

### 3.3.26.1. 0018-Improve-check-for-.-and-guard-against-dash-args.patch
Source: upstream

Size: 1.2K

SHA-512 Sum: 9960440da4d1ebd4f9c283f2a1d6f51cf6baf3d66a6f87b9a6da75aa4f23c9283
66ec6186d04b59ff0759934f463044399d1a6585b0f3e23f8eb94fd757c6fd3

### 3.3.26.1. 0019-Reject-log-file-when-read-only.patch
Source: upstream

Size: 632B

SHA-512 Sum: 58f737edcd65e51004f160052c7334b36611ebf5d97631fbd87ce48da34e26c4d
b0d7a04a7aa83907876e95ee5d97f5a94dd96698fda5ece58a6327ed0334ac9

### 3.3.26.1. 0020-Fix-prealloc-to-keep-file-size-0-when-possible.patch
Source: upstream

Size: 761B

SHA-512 Sum: 05ae005539778ed9a4384145a70ebf3ae4853318e09e0feb83ccc96c5ac8f6a1a
aab78b84b221ed32043ba6a7bd2a9168b5caa5dc7cfdb079237ed493d8beb4d

### 3.3.26.1. 0021-Avoid-leaving-a-file-open-on-error-return.patch
Source: upstream

Size: 660B

SHA-512 Sum: 16ee71e2511b40e04f16df427f1826eff03e6dbe299f866af834e0dc359be3baf
c3247010c0185c61a1cb01f2d784f71efd050e92c6fa306c747e3fa97971f30

### 3.3.26.1. 0022-Avoid-warning-about-leaked-mem-didn-t-affect-rsync-s.patch
Source: upstream

Size: 906B

SHA-512 Sum: 7fd3144cec8518203c8c73c04211e55ada504b32b69bc6294981df092a36b7ecd
d88eb11f49c7bb71a1ac3d6904dedb16c6de7385f8e78f96a049527f1ed2e6f

### 3.3.26.1. 0023-Use-a-separate-pass-by-value-pointer-for-clarity.patch
Source: upstream

Size: 0.9K

SHA-512 Sum: 17a88daf65cc5807f6d03281c2bf8e5f641933f8d70b27a2ef902081016066814
161b24260ddbf09c8d460e7c488d6be6ec79dcfd9fba640c87c9a4e45b959cb

### 3.3.26.1. 0024-Update-option-culling-to-handle-latest-changes.patch
Source: upstream

Size: 1.4K

SHA-512 Sum: 0b91061f432746978fdf5e009c0e562933d470b56290c1ea420e272e5f28a330d
07a5c59927f2bff82211ed004464a0b530ea7fb4f86b7b84a51d92a42a841c7

### 3.3.26.1. 0025-Improve-write-only-sender-check-handle-2-new-options.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: d29a10abc838346d94e8bb5c257bc8618b14e444c8122ad7c78be0b6123ba1ce7
785de4c2d4f379b5d50b7b1a6a2c4159277eef24ab8abf5b54d00811dc0c88d

### 3.3.26.1. 0026-Handle-a-run-from-down-inside-the-checkout-tree.patch
Source: upstream

Size: 1.4K

SHA-512 Sum: 9d1957d240fc15703188d36cfd7a46fe5af03c5d0d6ce69b6c7f9db9b456bd425
df5a9d20b63d1e9c91be9ce885ad3aafedc654dad9c9cb1afe3a2cc2cbef7a1

### 3.3.26.1. 0027-Fix-remove-source-files-sanity-check-w-copy-links-th.patch
Source: upstream

Size: 1.3K

SHA-512 Sum: ec22623bd1b1bca0fd956c92d0b51a59903090b761fac01bda9dbe7a95734719b
dd11be568a9d80dbe4acbe67444b5d1a0fa0b5db5c8120b5cc889db2f2a2800

### 3.3.26.1. 0028-Tweak-the-copyright-year.patch
Source: upstream

Size: 27K

SHA-512 Sum: 299d7eb844f029509284e8ceef82dfb90c2f2b67579c7fd77c6b77d89563e2eed
1091aae453e4a63e000192b34a5741c8e0fe1db955f2e8e894ebafdf5fb3004

### 3.3.26.1. 0029-Fix-zlib-CVE-2016-9840.patch
Source: upstream

Size: 2.2K

SHA-512 Sum: b6c142af3470886c718f381947428f30f03cd7c6adbe69f44c6c31fa072b5da2b
e168f4b08ef4dc9666aaed5f4807e74dd4ff9424677a87c741d089bbbb7be86

### 3.3.26.1. 0030-Fix-zlib-CVE-2016-9841.patch
Source: upstream

Size: 9.0K

SHA-512 Sum: a482ba60c49a0db59413311cbdfb084bc440a3cd098b5a4af43277b912f6dfc98
16301bd707d881e5f7a32b588ba0ff3354c6eb818e475064cacd7b85f497383

### 3.3.26.1. 0031-Fix-zlib-CVE-2016-9842.patch
Source: upstream

Size: 946B

SHA-512 Sum: 210ffa9902b3c46e4c9f3f49b57d12962f8fb9b6a0ea0339c8bb1ed427e486281
e44b250f7dfdc27ff0d2d0dc294a0ed8b17c593c672bf9202c425774956add9

### 3.3.26.1. 0032-Fix-zlib-CVE-2016-9843.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: d20e2f4fa58a219a735c1a2b48fae5b283ce2011ef2550dda3cf29504c604629f
49bda6ad2ffecabf348b278fc7b06e919959b27a16fa15f757ab6c6fa75fe05

### 3.3.26.1. 0033-Some-doc-tweaks-suggested-by-Cl-ment-Pit-Claudel.patch
Source: upstream

Size: 2.0K

SHA-512 Sum: 57b10483d5aa2b393700cf39d372365e64ea770b783f7a7c8a4c7256d9a640123
ec1a93a25e0c402fa0058f5ea5f21e48f17093d0bedfe89e7813532c36efaa9

### 3.3.26.1. 0034-Clarify-the-cut-off-point-for-copy-safe-links.patch
Source: upstream

Size: 1.1K

SHA-512 Sum: a72bf4290163cc561310590a0916f968232de5c00f5f3a27d3e57bdf0c122ea7a
1228b53e28a0a2d644ca68e04240bd0d154619c97df7f10c1b1bb2cf24a9dfd

### 3.3.26.1. 0035-Fix-bug-in-try_dests_reg-that-Florian-Zumbiehl-point.patch
Source: upstream

Size: 1.5K

SHA-512 Sum: 27f38529e67b882933ab24695e64deefe84db5b43ad1c1b2fec71ec44d3d52a00
ab3526e1cb69211832cb8363863f0a822ef60995d5a12002d4844a00b58ef18

### 3.3.26.1. 0036-Try-to-fix-the-iconv-crash-in-bug-11338.patch
Source: upstream

Size: 1.0K

SHA-512 Sum: 5af09f6a7660dba217251fbf386294cf9538d5a9554d2f4544e83d26fff7ac40e
eec556c2cdfa118d0feceb5aeb4413a7931710a0153f037b113f9f713cbd121

## 3.3.27. samurai
### 3.3.27.1. 0001-Fix-manifest-rebuild-when-it-was-pruned-due-to-resta.patch
Source: michaelforney

Size: 2.1K

SHA-512 Sum: ce44e1be76ed724945e6b59d9e5d778ba2652dbf011f623068ed569f6c9384c00
033ffaf3f0e789c0bfc029a9ac96cebf504b777ac2f86db8a45c3358ec6e955

### 3.3.27.1. 0002-parse-Check-that-rules-always-have-a-command.patch
Source: michaelforney

Size: 1.3K

SHA-512 Sum: 9bb40106e9c421c342ffa0fbc43b6c2b57004b3958a5d1feea7c3fdc708b502c7
1d39b231147e6c036c5b84a9a31feb240dc3f55d230ac0725245c6b93072a6a

### 3.3.27.1. 0003-parse-Check-that-rules-have-rspfile-iff-they-have-rs.patch
Source: michaelforney

Size: 1.5K

SHA-512 Sum: 9107ff0a8a76dd79737b7f7bd2dd3507d990df912236dea3cf186ad800da8ec66
a109df116682b9e47e33c67a1a57803b8cab9a29df29763609b484a6b153c41

### 3.3.27.1. 0004-tool-Implement-compdb.patch
Source: michaelforney

Size: 4.2K

SHA-512 Sum: 3d01d9b529e95e0363d2bd104d30b9f234ff8986509b469a6c9ed79aa4d06c11a
9bbc49b57833e4757a561240683c788cb328a68381e89c73876d23234000b18

### 3.3.27.1. 0005-compdb-Remove-trailing-comma-after-last-entry-in-com.patch
Source: michaelforney

Size: 640B

SHA-512 Sum: bcb6b6a144782ed219a9be0c10f7abf784087afed916f6c6504d66740f7bec28a
636035afcbb4ce58f1e9e1357b4a43e2b8501784571e9d0c372f13579c5d316

### 3.3.27.1. 0006-Add-support-for-NINJA_STATUS-environment-variable.patch
Source: michaelforney

Size: 4.6K

SHA-512 Sum: 487e553cbb174167eb26f6321ca1d50798d50eae0b03c03ee16be5d3f95b1d825
92aa0c22ee049ad48cdc07f25ba4cd959dcb011b7bcbd401d19bf101416dd8f

### 3.3.27.1. 0007-manual-Specify-list-width-to-avoid-lint-warning.patch
Source: michaelforney

Size: 642B

SHA-512 Sum: 17087c175d00f985c73e9192fecee947727ae9db579a4cfa04c0bb2d6a7b6b478
64bb6e93bf0253a43290b6b9a131c33041084cb5f587b96d3e21b873419eb1b

## 3.3.28. shadow
### 3.3.28.1. 0001-change-default-shell.patch
Source: glaucus

Size: 158B

SHA-512 Sum: 50ca2e705e31dea9f97252b643e9656a7fa1d6dea894f883dd8acac20f6a4717f
88c6c38509ecbed523e18a4c0694fa4d02c5bd8456ddc1da0bbea91a8524740

### 3.3.28.1. 0002-fix-installation-paths.patch
Source: glaucus

Size: 207B

SHA-512 Sum: 5ae18bd9070bbf9b2e298e6fae623349f325041dd97bdce349221b9503685c934
bcf3b80af505daa1d85d924f6febf8df7e2254f434d8398c4c79174c4649cd2

## 3.3.29. texinfo
### 3.3.29.1. fix-build-without-NLS.patch
Source: alpine

Size: 511B

SHA-512 Sum: 1c33d8c8bf24ec139fa2a283e12d42a260027d354061d348b66f1d2ef4636573c
b88442299595af946366c9e9cc5511450a32d1a1fb827bee30f38a7558b3edb

## 3.3.30. xz
### 3.3.30.1. add-pgo.patch
Source: clear

Size: 751B

SHA-512 Sum: 217175c6f6d518ac1bbc09c23040c349b15e357a0bdce3dad10c42e3acac6df06
18a0bd0eeaeeeaf00008342c6861372f535b9891d69a629f81256d933373368

### 3.3.30.1. default-threading.patch
Source: clear

Size: 276B

SHA-512 Sum: 17c45c46ec31148406b179a6a9fc435abdb3211935a339546b5cff6ab3c93b5d6
063df43668e2d772c6d3685f5ca77e608f559af02fb1964e7b13c09af2f265c

### 3.3.30.1. io-size.patch
Source: clear

Size: 316B

SHA-512 Sum: c0505463179655e6bdac1f82432c4ff184d849967c94aad3f8c2300fcf000d664
19a82511f8f1372f6cce58c0df5f46ae55f1b001b226944c5c8d984121f1c63

### 3.3.30.1. speedup.patch
Source: clear

Size: 1.0K

SHA-512 Sum: b2515dd55ef701951e5c38de522850340ede641411bf3ef52cd290f5e4c8ba5fc
b43c563d0a762da9ce7b7656c8381b55667f3e419b39809b8bbf80f626caa1e
