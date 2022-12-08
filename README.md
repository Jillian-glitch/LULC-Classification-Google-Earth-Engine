# LULC-Classification-Google-Earth-Engine
var roi = ee.FeatureCollection("users/jillianwangari98/uppertana"),
    snow = /* color: #0dc8d6 */ee.FeatureCollection(
        [ee.Feature(
            ee.Geometry.Point([37.312076820143076, -0.1545346312545017]),
            {
              "landcover": 0,
              "system:index": "0"
            }),
        ee.Feature(
            ee.Geometry.Point([37.314093841322276, -0.15535001981355825]),
            {
              "landcover": 0,
              "system:index": "1"
            }),
        ee.Feature(
            ee.Geometry.Point([37.315853370436045, -0.15483503756937295]),
            {
              "landcover": 0,
              "system:index": "2"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31593920112452, -0.1564658146328187]),
            {
              "landcover": 0,
              "system:index": "3"
            }),
        ee.Feature(
            ee.Geometry.Point([37.3149092328628, -0.15556459574492057]),
            {
              "landcover": 0,
              "system:index": "4"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31516672492823, -0.1573670334819904]),
            {
              "landcover": 0,
              "system:index": "5"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31641126991114, -0.15762452457460566]),
            {
              "landcover": 0,
              "system:index": "6"
            }),
        ee.Feature(
            ee.Geometry.Point([37.315595878370615, -0.15818242193103793]),
            {
              "landcover": 0,
              "system:index": "7"
            }),
        ee.Feature(
            ee.Geometry.Point([37.315381301649424, -0.15856865855361915]),
            {
              "landcover": 0,
              "system:index": "8"
            }),
        ee.Feature(
            ee.Geometry.Point([37.3145659101089, -0.15904072552700046]),
            {
              "landcover": 0,
              "system:index": "9"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31675459266505, -0.15547876537263264]),
            {
              "landcover": 0,
              "system:index": "10"
            }),
        ee.Feature(
            ee.Geometry.Point([37.312849296339365, -0.1551783590668832]),
            {
              "landcover": 0,
              "system:index": "11"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31353594184718, -0.1565516450010737]),
            {
              "landcover": 0,
              "system:index": "12"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31130434394679, -0.1553929350000012]),
            {
              "landcover": 0,
              "system:index": "13"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31177641273341, -0.15535001981355825]),
            {
              "landcover": 0,
              "system:index": "14"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31675459266505, -0.15281802365966393]),
            {
              "landcover": 0,
              "system:index": "15"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31864286781153, -0.15354758190431866]),
            {
              "landcover": 0,
              "system:index": "16"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31829954505763, -0.15659456018507398]),
            {
              "landcover": 0,
              "system:index": "17"
            }),
        ee.Feature(
            ee.Geometry.Point([37.318857444532725, -0.15659456018507398]),
            {
              "landcover": 0,
              "system:index": "18"
            })]),
    forest = /* color: #3e6800 */ee.FeatureCollection(
        [ee.Feature(
            ee.Geometry.Point([37.17798994915032, -0.10145380425555348]),
            {
              "landcover": 1,
              "system:index": "0"
            }),
        ee.Feature(
            ee.Geometry.Point([37.17798994915032, -0.11381340156373686]),
            {
              "landcover": 1,
              "system:index": "1"
            }),
        ee.Feature(
            ee.Geometry.Point([37.16391371624017, -0.11484336777495033]),
            {
              "landcover": 1,
              "system:index": "2"
            }),
        ee.Feature(
            ee.Geometry.Point([37.21403883831048, -0.054418631804870436]),
            {
              "landcover": 1,
              "system:index": "3"
            }),
        ee.Feature(
            ee.Geometry.Point([37.22159193889642, -0.05991179313119389]),
            {
              "landcover": 1,
              "system:index": "4"
            }),
        ee.Feature(
            ee.Geometry.Point([37.20236586467767, -0.06059843825929793]),
            {
              "landcover": 1,
              "system:index": "5"
            }),
        ee.Feature(
            ee.Geometry.Point([37.21472548381829, -0.06334501868370178]),
            {
              "landcover": 1,
              "system:index": "6"
            }),
        ee.Feature(
            ee.Geometry.Point([37.20511244670892, -0.06574827643585114]),
            {
              "landcover": 1,
              "system:index": "7"
            }),
        ee.Feature(
            ee.Geometry.Point([37.21884535686517, -0.0722714040250021]),
            {
              "landcover": 1,
              "system:index": "8"
            }),
        ee.Feature(
            ee.Geometry.Point([37.23841475383782, -0.0369091769846641]),
            {
              "landcover": 1,
              "system:index": "9"
            }),
        ee.Feature(
            ee.Geometry.Point([37.22433852092767, -0.034849240865224014]),
            {
              "landcover": 1,
              "system:index": "10"
            }),
        ee.Feature(
            ee.Geometry.Point([37.214382161064385, -0.03278930470074728]),
            {
              "landcover": 1,
              "system:index": "11"
            }),
        ee.Feature(
            ee.Geometry.Point([37.19996260540032, -0.042402339729362276]),
            {
              "landcover": 1,
              "system:index": "12"
            }),
        ee.Feature(
            ee.Geometry.Point([37.19137953655267, -0.04995543785660418]),
            {
              "landcover": 1,
              "system:index": "13"
            }),
        ee.Feature(
            ee.Geometry.Point([37.1766166581347, -0.04789550208428984]),
            {
              "landcover": 1,
              "system:index": "14"
            }),
        ee.Feature(
            ee.Geometry.Point([37.23807143108392, -0.06094176082009306]),
            {
              "landcover": 1,
              "system:index": "15"
            })]),
    vegetation = /* color: #0ae016 */ee.FeatureCollection(
        [ee.Feature(
            ee.Geometry.Point([37.502689107283516, -0.12319559223448988]),
            {
              "landcover": 2,
              "system:index": "0"
            }),
        ee.Feature(
            ee.Geometry.Point([37.49479268394367, -0.13898839752733647]),
            {
              "landcover": 2,
              "system:index": "1"
            }),
        ee.Feature(
            ee.Geometry.Point([37.48105977378742, -0.15169129852646573]),
            {
              "landcover": 2,
              "system:index": "2"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46767018638508, -0.1561544782205164]),
            {
              "landcover": 2,
              "system:index": "3"
            }),
        ee.Feature(
            ee.Geometry.Point([37.48655293784992, -0.16611079869885828]),
            {
              "landcover": 2,
              "system:index": "4"
            }),
        ee.Feature(
            ee.Geometry.Point([37.3917958577718, -0.11770244031227783]),
            {
              "landcover": 2,
              "system:index": "5"
            }),
        ee.Feature(
            ee.Geometry.Point([37.407588704451484, -0.13658514519945775]),
            {
              "landcover": 2,
              "system:index": "6"
            }),
        ee.Feature(
            ee.Geometry.Point([37.423038228377266, -0.13246528350921796]),
            {
              "landcover": 2,
              "system:index": "7"
            }),
        ee.Feature(
            ee.Geometry.Point([37.41788838706867, -0.14688479628887127]),
            {
              "landcover": 2,
              "system:index": "8"
            }),
        ee.Feature(
            ee.Geometry.Point([37.51333211265461, -0.09126663245237003]),
            {
              "landcover": 2,
              "system:index": "9"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46080373130695, -0.18842667075349817]),
            {
              "landcover": 2,
              "system:index": "10"
            }),
        ee.Feature(
            ee.Geometry.Point([37.58096669517414, -0.08199692870309938]),
            {
              "landcover": 2,
              "system:index": "11"
            }),
        ee.Feature(
            ee.Geometry.Point([37.58817647300617, -0.09572982230941246]),
            {
              "landcover": 2,
              "system:index": "12"
            }),
        ee.Feature(
            ee.Geometry.Point([37.61461232505695, -0.12834542113409025]),
            {
              "landcover": 2,
              "system:index": "13"
            }),
        ee.Feature(
            ee.Geometry.Point([37.62559865318195, -0.14345157977001652]),
            {
              "landcover": 2,
              "system:index": "14"
            }),
        ee.Feature(
            ee.Geometry.Point([37.716922505721016, -0.1314353179788213]),
            {
              "landcover": 2,
              "system:index": "15"
            }),
        ee.Feature(
            ee.Geometry.Point([37.68602345786945, -0.16405087072563296]),
            {
              "landcover": 2,
              "system:index": "16"
            }),
        ee.Feature(
            ee.Geometry.Point([37.6664540608968, -0.14139164961069417]),
            {
              "landcover": 2,
              "system:index": "17"
            }),
        ee.Feature(
            ee.Geometry.Point([37.68053029380695, -0.10705945542915155]),
            {
              "landcover": 2,
              "system:index": "18"
            })]),
    water = /* color: #372fff */ee.FeatureCollection(
        [ee.Feature(
            ee.Geometry.Point([37.46334447407129, -0.5573381124280906]),
            {
              "landcover": 3,
              "system:index": "0"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46366633915308, -0.55755267899361]),
            {
              "landcover": 3,
              "system:index": "1"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46457829021814, -0.557617048961734]),
            {
              "landcover": 3,
              "system:index": "2"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46488942646387, -0.5575097656811244]),
            {
              "landcover": 3,
              "system:index": "3"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46557607197168, -0.5572201008137142]),
            {
              "landcover": 3,
              "system:index": "4"
            }),
        ee.Feature(
            ee.Geometry.Point([37.466273446315554, -0.5572522857996846]),
            {
              "landcover": 3,
              "system:index": "5"
            }),
        ee.Feature(
            ee.Geometry.Point([37.4666596844137, -0.5574239390552246]),
            {
              "landcover": 3,
              "system:index": "6"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46718539738062, -0.5577565172236068]),
            {
              "landcover": 3,
              "system:index": "7"
            }),
        ee.Feature(
            ee.Geometry.Point([37.463022608989505, -0.5569089792736049]),
            {
              "landcover": 3,
              "system:index": "8"
            }),
        ee.Feature(
            ee.Geometry.Point([37.462732930415896, -0.5562116378309251]),
            {
              "landcover": 3,
              "system:index": "9"
            }),
        ee.Feature(
            ee.Geometry.Point([37.4626256420553, -0.5557825045944828]),
            {
              "landcover": 3,
              "system:index": "10"
            }),
        ee.Feature(
            ee.Geometry.Point([37.462797303432254, -0.5563940194469741]),
            {
              "landcover": 3,
              "system:index": "11"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46733560108545, -0.5578208871895172]),
            {
              "landcover": 3,
              "system:index": "12"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46763600849512, -0.5579603554465555]),
            {
              "landcover": 3,
              "system:index": "13"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46779694103601, -0.5580461820646312]),
            {
              "landcover": 3,
              "system:index": "14"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31717345316898, -0.17144967794297197]),
            {
              "landcover": 3,
              "system:index": "15"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31580016215335, -0.1678877199895225]),
            {
              "landcover": 3,
              "system:index": "16"
            }),
        ee.Feature(
            ee.Geometry.Point([37.31502768595706, -0.16638568933192932]),
            {
              "landcover": 3,
              "system:index": "17"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32828852732669, -0.16694358644671575]),
            {
              "landcover": 3,
              "system:index": "18"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32923266489993, -0.1679735503093313]),
            {
              "landcover": 3,
              "system:index": "19"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33082053263675, -0.16926100506123565]),
            {
              "landcover": 3,
              "system:index": "20"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33258006175052, -0.1706342900357001]),
            {
              "landcover": 3,
              "system:index": "21"
            }),
        ee.Feature(
            ee.Geometry.Point([37.333223791914094, -0.17127801733379866]),
            {
              "landcover": 3,
              "system:index": "22"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33403918345462, -0.17187882945916882]),
            {
              "landcover": 3,
              "system:index": "23"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33459708292972, -0.1724367264158181]),
            {
              "landcover": 3,
              "system:index": "24"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33511206706058, -0.17282296276083864]),
            {
              "landcover": 3,
              "system:index": "25"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33601328928958, -0.1736812657216444]),
            {
              "landcover": 3,
              "system:index": "26"
            }),
        ee.Feature(
            ee.Geometry.Point([37.3370432575513, -0.1745395686434693]),
            {
              "landcover": 3,
              "system:index": "27"
            }),
        ee.Feature(
            ee.Geometry.Point([37.328696223096955, -0.17653512278498543]),
            {
              "landcover": 3,
              "system:index": "28"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32815978129398, -0.17571973509699373]),
            {
              "landcover": 3,
              "system:index": "29"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32777354319583, -0.17501163523378466]),
            {
              "landcover": 3,
              "system:index": "30"
            }),
        ee.Feature(
            ee.Geometry.Point([37.326679201917756, -0.17325211424610779]),
            {
              "landcover": 3,
              "system:index": "31"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32588526804935, -0.1728015051863252]),
            {
              "landcover": 3,
              "system:index": "32"
            }),
        ee.Feature(
            ee.Geometry.Point([37.3254990299512, -0.17245818399073864]),
            {
              "landcover": 3,
              "system:index": "33"
            })]),
    urban = /* color: #b8bdd8 */ee.FeatureCollection(
        [ee.Feature(
            ee.Geometry.Point([37.46439590000513, -0.5562223661614351]),
            {
              "landcover": 4,
              "system:index": "0"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46429934048059, -0.5560828978632658]),
            {
              "landcover": 4,
              "system:index": "1"
            }),
        ee.Feature(
            ee.Geometry.Point([37.4645890190542, -0.5564262044374481]),
            {
              "landcover": 4,
              "system:index": "2"
            }),
        ee.Feature(
            ee.Geometry.Point([37.45966448330286, -0.5591511996604066]),
            {
              "landcover": 4,
              "system:index": "3"
            }),
        ee.Feature(
            ee.Geometry.Point([37.45997561954859, -0.5590224597570327]),
            {
              "landcover": 4,
              "system:index": "4"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46117017637876, -0.5611987249255161]),
            {
              "landcover": 4,
              "system:index": "5"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46115676533368, -0.5612684590142974]),
            {
              "landcover": 4,
              "system:index": "6"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46107629906324, -0.5612416382110179]),
            {
              "landcover": 4,
              "system:index": "7"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46120504509595, -0.5610753492279366]),
            {
              "landcover": 4,
              "system:index": "8"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46171466480878, -0.560482609427241]),
            {
              "landcover": 4,
              "system:index": "9"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46205262314466, -0.5605416152019368]),
            {
              "landcover": 4,
              "system:index": "10"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46093950640348, -0.5604691990238074]),
            {
              "landcover": 4,
              "system:index": "11"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46008656393674, -0.5606193955404166]),
            {
              "landcover": 4,
              "system:index": "12"
            }),
        ee.Feature(
            ee.Geometry.Point([37.459984639994175, -0.5605952568147934]),
            {
              "landcover": 4,
              "system:index": "13"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46004901301053, -0.560563071847143]),
            {
              "landcover": 4,
              "system:index": "14"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46008656393674, -0.5609331989644609]),
            {
              "landcover": 4,
              "system:index": "15"
            }),
        ee.Feature(
            ee.Geometry.Point([37.45988271605161, -0.5610994879515879]),
            {
              "landcover": 4,
              "system:index": "16"
            }),
        ee.Feature(
            ee.Geometry.Point([37.459968546740086, -0.561061938825877]),
            {
              "landcover": 4,
              "system:index": "17"
            }),
        ee.Feature(
            ee.Geometry.Point([37.459721783510716, -0.5611719041219185]),
            {
              "landcover": 4,
              "system:index": "18"
            }),
        ee.Feature(
            ee.Geometry.Point([37.4604218400636, -0.5604101932483738]),
            {
              "landcover": 4,
              "system:index": "19"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46317378651288, -0.5619550715363599]),
            {
              "landcover": 4,
              "system:index": "20"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46318719755796, -0.5618397420949292]),
            {
              "landcover": 4,
              "system:index": "21"
            }),
        ee.Feature(
            ee.Geometry.Point([37.463120142332585, -0.5618611987353773]),
            {
              "landcover": 4,
              "system:index": "22"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46314428221372, -0.5616841814494059]),
            {
              "landcover": 4,
              "system:index": "23"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46250323425916, -0.5617378230517794]),
            {
              "landcover": 4,
              "system:index": "24"
            }),
        ee.Feature(
            ee.Geometry.Point([37.462522009722264, -0.5617673259328807]),
            {
              "landcover": 4,
              "system:index": "25"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46397844921735, -0.5616385860869986]),
            {
              "landcover": 4,
              "system:index": "26"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46406696211484, -0.5616519964877478]),
            {
              "landcover": 4,
              "system:index": "27"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46670357357648, -0.5621776841726908]),
            {
              "landcover": 4,
              "system:index": "28"
            }),
        ee.Feature(
            ee.Geometry.Point([37.466727713457615, -0.5621937766520886]),
            {
              "landcover": 4,
              "system:index": "29"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46666870485929, -0.5621830483324942]),
            {
              "landcover": 4,
              "system:index": "30"
            }),
        ee.Feature(
            ee.Geometry.Point([37.4668510950723, -0.5622071870515656]),
            {
              "landcover": 4,
              "system:index": "31"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46686718832639, -0.5622474182497931]),
            {
              "landcover": 4,
              "system:index": "32"
            }),
        ee.Feature(
            ee.Geometry.Point([37.467269519678624, -0.5621937766520886]),
            {
              "landcover": 4,
              "system:index": "33"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46725610863355, -0.5621991408118794]),
            {
              "landcover": 4,
              "system:index": "34"
            }),
        ee.Feature(
            ee.Geometry.Point([37.467468003145726, -0.5620704009755134]),
            {
              "landcover": 4,
              "system:index": "35"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46770135533002, -0.5619121582560997]),
            {
              "landcover": 4,
              "system:index": "36"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46792397867826, -0.5619684819363839]),
            {
              "landcover": 4,
              "system:index": "37"
            }),
        ee.Feature(
            ee.Geometry.Point([37.467894474379094, -0.5619362969762907]),
            {
              "landcover": 4,
              "system:index": "38"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46642194162992, -0.5624432100771957]),
            {
              "landcover": 4,
              "system:index": "39"
            }),
        ee.Feature(
            ee.Geometry.Point([37.4664004839578, -0.5624539383963192]),
            {
              "landcover": 4,
              "system:index": "40"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46656946312574, -0.5625075799916192]),
            {
              "landcover": 4,
              "system:index": "41"
            })]),
    bareland = /* color: #764d33 */ee.FeatureCollection(
        [ee.Feature(
            ee.Geometry.Point([37.470713476053746, -0.562966215611355]),
            {
              "landcover": 5,
              "system:index": "0"
            }),
        ee.Feature(
            ee.Geometry.Point([37.470608869902165, -0.5628964815428402]),
            {
              "landcover": 5,
              "system:index": "1"
            }),
        ee.Feature(
            ee.Geometry.Point([37.4706517852464, -0.5629635335318031]),
            {
              "landcover": 5,
              "system:index": "2"
            }),
        ee.Feature(
            ee.Geometry.Point([37.47101656567243, -0.5636742845674604]),
            {
              "landcover": 5,
              "system:index": "3"
            }),
        ee.Feature(
            ee.Geometry.Point([37.47104070555356, -0.5637198799139523]),
            {
              "landcover": 5,
              "system:index": "4"
            }),
        ee.Feature(
            ee.Geometry.Point([37.47084758650449, -0.5636957412011403]),
            {
              "landcover": 5,
              "system:index": "5"
            }),
        ee.Feature(
            ee.Geometry.Point([37.470759073607, -0.5634409436709734]),
            {
              "landcover": 5,
              "system:index": "6"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46585304174584, -0.5655812777969206]),
            {
              "landcover": 5,
              "system:index": "7"
            }),
        ee.Feature(
            ee.Geometry.Point([37.465922779180225, -0.565785115746914]),
            {
              "landcover": 5,
              "system:index": "8"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46581549081963, -0.565055590419181]),
            {
              "landcover": 5,
              "system:index": "9"
            }),
        ee.Feature(
            ee.Geometry.Point([37.465912050344166, -0.5650394979476837]),
            {
              "landcover": 5,
              "system:index": "10"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46628755960625, -0.5655169079164908]),
            {
              "landcover": 5,
              "system:index": "11"
            }),
        ee.Feature(
            ee.Geometry.Point([37.4663143816964, -0.5655920061102555]),
            {
              "landcover": 5,
              "system:index": "12"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46611053381127, -0.5651628735613602]),
            {
              "landcover": 5,
              "system:index": "13"
            }),
        ee.Feature(
            ee.Geometry.Point([37.46636266145867, -0.5648356599715205]),
            {
              "landcover": 5,
              "system:index": "14"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32376095850955, -0.17511892309356605]),
            {
              "landcover": 5,
              "system:index": "15"
            }),
        ee.Feature(
            ee.Geometry.Point([37.324447604017365, -0.1758913956658376]),
            {
              "landcover": 5,
              "system:index": "16"
            }),
        ee.Feature(
            ee.Geometry.Point([37.326443167524445, -0.17696427418538466]),
            {
              "landcover": 5,
              "system:index": "17"
            }),
        ee.Feature(
            ee.Geometry.Point([37.321422072248566, -0.17383146873578334]),
            {
              "landcover": 5,
              "system:index": "18"
            }),
        ee.Feature(
            ee.Geometry.Point([37.322430582838166, -0.17387438388245663]),
            {
              "landcover": 5,
              "system:index": "19"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32200142939578, -0.17591285323683972]),
            {
              "landcover": 5,
              "system:index": "20"
            }),
        ee.Feature(
            ee.Geometry.Point([37.324211569624055, -0.1773290528679049]),
            {
              "landcover": 5,
              "system:index": "21"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32725855906497, -0.17818735562193647]),
            {
              "landcover": 5,
              "system:index": "22"
            }),
        ee.Feature(
            ee.Geometry.Point([37.32959744532596, -0.17878816752597818]),
            {
              "landcover": 5,
              "system:index": "23"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33436104853641, -0.17432499291668027]),
            {
              "landcover": 5,
              "system:index": "24"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33712908823978, -0.17702864689458706]),
            {
              "landcover": 5,
              "system:index": "25"
            }),
        ee.Feature(
            ee.Geometry.Point([37.33828780253421, -0.17786549209385005]),
            {
              "landcover": 5,
              "system:index": "26"
            }),
        ee.Feature(
            ee.Geometry.Point([37.345390292005646, -0.17254401429021732]),
            {
              "landcover": 5,
              "system:index": "27"
            }),
        ee.Feature(
            ee.Geometry.Point([37.345948191480744, -0.17398167174872636]),
            {
              "landcover": 5,
              "system:index": "28"
            })]);
Map.addLayer(roi,{},'uppertana',true);
var roi = ee.FeatureCollection("users/jillianwangari98/uppertana");
/**
 * Function to mask clouds based on the pixel_qa band of Landsat SR data.
 * @param {ee.Image} image Input Landsat SR image
 * @return {ee.Image} Cloudmasked Landsat image
 */
var cloudMaskL457 = function(image) {
  var qa = image.select('pixel_qa');
  // If the cloud bit (5) is set and the cloud confidence (7) is high
  // or the cloud shadow bit is set (3), then it's a bad pixel.
  var cloud = qa.bitwiseAnd(1 << 5)
                  .and(qa.bitwiseAnd(1 << 7))
                  .or(qa.bitwiseAnd(1 << 3));
  // Remove edge pixels that don't occur in all bands
  var mask2 = image.mask().reduce(ee.Reducer.min());
  return image.updateMask(cloud.not()).updateMask(mask2);
};

var imagery = ee.ImageCollection('LANDSAT/LE07/C01/T1_SR')
                  .filterDate('2005-05-01', '2007-07-31')
                  .map(cloudMaskL457);

var visParams = {
  bands: ['B3', 'B2', 'B1'],
  min: 0,
  max: 3000,
  gamma: 1.4,
};
Map.centerObject(roi, 10);
var uppertana=imagery.median().clip(roi)
Map.addLayer(uppertana, visParams);
// Merge the three geometry layers into a single FeatureCollection.
var newfc = snow.merge(bareland).merge(Water).merge(forest).merge(vegetation).merge(urban);
var label = 'landcover'
var bands = ['B1', 'B2', 'B3', 'B4', 'B5', 'B6','B7']
var sample = uppertana.select(bands).sampleRegions({
  'collection': newfc,
  'properties': [label],
  'scale': 30
})
var Sample = sample.randomColumn()

var split = 0.7

var training = Sample.filter(ee.Filter.lt('random', split))
var validation = Sample.filter(ee.Filter.gte('random', split))

//Train a randomforest classifier with default parameters.
var classifier = ee.Classifier.smileRandomForest(10).train(training, label, bands)
//Classify the image with the same bands used for training.
var result = uppertana.select(bands).classify(classifier)
Map.addLayer(result.randomVisualizer(), {}, 'classfied')
var train_accuracy = classifier.confusionMatrix()
print('confusionMatrix',train_accuracy)
print('Overallaccuraccy',train_accuracy.accuracy())
print('kappa',train_accuracy.kappa())
//Export results
Export.image.toDrive({
image: result,
description: 'Classified2018',
scale: 30,
region: roi,
});s.
