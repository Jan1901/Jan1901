
--[[
AztupBrew(Fork of IronBrew2): obfuscation; Version 2.7.2
]]
return(function(h,a,o)local k=string.char;local e=string.sub;local m=table.concat;local n=math.ldexp;local t=getfenv or function()return _ENV end;local l=select;local g=unpack or table.unpack;local i=tonumber;local function p(h)local b,c,f="","",{}local d=256;local g={}for a=0,d-1 do g[a]=k(a)end;local a=1;local function j()local b=i(e(h,a,a),36)a=a+1;local c=i(e(h,a,a+b-1),36)a=a+b;return c end;b=k(j())f[1]=b;while a<#h do local a=j()if g[a]then c=g[a]else c=b..e(b,1,1)end;g[d]=b..e(c,1,1)f[#f+1],b,d=c,c,d+1 end;return table.concat(f)end;local j=p('21Q23827523B2342752381J1L1P1H23B2372792101O1L1D1H161723B23J27921K1R1N1L1O27I27K27M23B235279141L1T27N23B23H27H27J27L1621F111T27P27921F1H1021J1S1T1O1G161H1Q27727921M27C27E2882752131N28Q28R28D28F27G27521C1H1710161R1D23B23G27921P1Q29A1L1Q1N27E23B2791Q1H132802792131R111Q1G29U27521L11171T1N23B23627H1L28Q1Q1028727928L2AB1L1N1027Z22S27921O111P29L1R1T1G2121R1R102102AB2AE29623829W29Y1G21P2A022R279161M1C1L171728J2AU22622J22J21T21X21S2BO21Y21X21V21W2252A82791Y1R1O2AQ1H2792C323G21G28T27527X29E28127521E1628W2AF2751W1H1C1021K1L1M1H1O23B23I2792CI2CK21I1110101R1Q2C32D223B23C2791Z2841021E1R1628L28N2A02AN27521I2AJ1V1J29C2B621J2BZ2DB21Z2BW2752DO1O2DQ27F2791I29C1P21221F21I2D22382441R2C629G2C81R2A5101T2D02A12381X21C1T1P21Y2E523822O21G2EO22O2502C72B41T1E2C22E51T2ER2D2250162C622Q2792DI1N2DK2DM29Z1W2CE29J2832AC1N1D2EO23O2232EO21M2C62782CC2D02AE2FR23821D1Q2AQ29F27921H2AR2EE1N21321J2EV2CU2AE2F72C829C1U1H2AK22C21821K22C22H22C21Q29L21Y22F2BO21S2242CR2CT2CJ28K2DP162DR2CS2CH2GW29027V1H1G23A2392G02H22CK2132EX2EZ2C326S21H2C627Q2HB101Z2CE14142H62EO21V2F22D221Z2HU2C321S2ER22T24Q23I25W26L26L24T2232EV2132CZ142EO21C2FQ27929A1R1423B22T27921L29X2BH2CW2CY2D021X21J1O2A61V2DX2751N2D029R2AK23822D25K22P21G21Z21Z2472I82FV2A32AL2EV1P2CX2C22I12I32I52592I82CB2B4102B12EO22G2C62JP29K162FU279132D82EO2442I82D52C828A27M1Y27V1129923B23E27921E1T29Z2KH27N28K28M28O2EV21F2BZ2A02JP2KA2C02HF27922R24521G2FV22O27923A23823B22P27921229L1G1R1P22C2132HQ1N1T27V2EX1L2EE2EG2FV27B27D2GU27528I1021327M122A627E2IL2752121H142IV27U2AL1G2IA2DB1L1J27E2K62382M21P2AY1H21D1228R1027O23D2F8111D21P2AL2E11H2MH2JF2H12382KK1H2LV162ML162EV2K11T1023826M2I52ND2JN2IY2382C927M27O2HK23827S27U27W2K82N62EA2382F91V2832FA2KE2KG2KI1G2KK29A2DD2KO2KF2751X1N28M1S1L22C21D27L1M27V1O2392FL2FN2E52282C62L22DT1O1H2AB29I2ML2AD2DB1D2MG2MI2EO2EO21W2792322P42P627523327922W2PA2PC2752PB2PE2PD23822X2792PJ2752PL23822Y2792PP27522Z2792PT2PS27922C2PX2PZ2752PY2Q12Q02382Q22Q52EO2Q622D2792QA2752QC23822E2792QG2752282792QK2OM2792292QO2QQ2752QP2QS2QR23822A2792QX27522B2792R127522M2792P32792EN2E522A2O623822J2382OJ2OJ23421C2792RE2OJ22U2PR2382L427522U2262RF2L52Q02RG23827822U2762382JP2792OJ29P2L42Q22RX2A92S82RU27G2Q22L42OJ2NS2RY2P12L42782OJ2L32RU2D22RQ2792S02RP23828Y2382SS29P2MZ2SN2SF2SW2752L429P2Q32ST2L427Q2SE2ST2D52TA2L42MP2TD2382KF2SS27823F2E52SK2ST2QZ2L42PB2OJ2AN2RI2PC2RH2RJ2QD2SO2EN2T12Q12PB2L42L42M021E2ST2SM2752TL2SQ2KG2ST2D22U02SO2TH29P2S02QP2OJ2SK2TX2382UL2RY2UO2RL2SW2U42RV2Q129G2UV2RZ2752782S32T32SI2S72V42L42SA2V723822V2Q72RV2L42SH2S62RU2SX2EP2E529P2U92382ME2VN2P12T523821R2792VU27521K2792VS2382TL2752VN2U72EO2VP2792B32EH28328527O2SV2AH2CE2AK2AM2AO2AQ2AS2AU2AW2AY2B02JY28G2LS28J2O428P28R2EV28V2LQ2JP2A32A52A72B329829A29C2FK2C32DG23821B2792XC2752XE2XB2XD2XI2XF2XJ2382142792XN2752XP2382152792XT2XK2752162791K2792XA22U2302S42E52VQ2SB2UM2VD2RX29P2Y82SI2Y52UC2TM2YE2752MP2OJ22C2242S22SI2812RB2YO2YK2382A92TU2YJ2RU22C21F2YO2782962PJ2812T12362R323829G2Y92YW2Z92SO2W72P12VZ2822ZI275152ZH2792W22E52W52E52ZF2752302SM2VS2ZW2792FV2ZZ2ZY31012V12792JP31052792A927531082YI2B32SV310D2792SV2MZ2NL310I2792ME2MP2752RC2RC2ZO310Q2ZN2Y1310T2752XA2XA2M0238310Y31102SR31122RR31132VB2792VC275311831162752OP2VK311C279311D2L7275311I238311K311K2GB2382BA2R42792R5311R27522H279311W311V311X3120311Z31222RD2R631252752R72383128312A312623821X279312E275312G312D312F312K312H312L2382R9312O2R8312R275312P312U312S23821Z27921T27921U31313133275313231353134238313623821V279313C275313E313B313D313I313F313J2382YN275313N313M279313P2252792RT275313V238313X313Z313U31412752272792202792212792OL2382HU314C279314D275314F23821H2G1314K275314J314M314L314I314P2E42DH2F8314U314T314W2NT314V23821J2AG31522DT2792UO21D279315727531592FW3158315D315A2UD2LS2AO27R315J2752742A22IM315O315N27521N27H315T2C8315U2NH315W21027921131603162275316131643163238316531682L8316B2M1316C2MF316E212316E21329V316K28Z2CT2791X316O316Q2O7316R2EI316T1Y2D62792182XZ317027521A2791L3174317627531752751G2792HF317D317C317F275317E2751I2DY317L317J317M238317K317N317R27A2791J317U317W275317V317Y317X317T2751S2793184318331852791T2791U318B318D275318C318F318E238318G2381V2791O2791P2792ZL2ZK2791R2BB318W27516318X2381127931922753194238122793198275319A31973199319E319B319F319D319G275132792X8238319N319N1E2792ZU2RR22K2Y52T62C32V62D32T22RU2FV2TA2752812TG310A2ST2W02W32ZH2FV2TH2YY2YN2A928127G2YR2A92KF2SG2UR27931AM2Q52Z031AH2SU2PM2YU2U82YU2R12OJ2882ZB2UO31B12UU2RU2MZ22C2QK2RX27Q2SS2L42ME2YF2ST2R72OJ27G2TF2V42UA2VD2UV2AN2DG2OJ2KF2L431BH310Z2T231BU2VC2L22TA2OJ311I2PJ2UV2RM2312ST31B72VA31BB2S12SH2VA2L42VJ31C82RV29P31CA2SI311O2ZH2UV2TJ23831CG27827831BB2PP281311Q2752IL27831CN31A531CP2Q028128131CJ2A92Y42D22Z52ST2SS2A931CG2A92A931CJ27G31D82C32A931D023827G31B72YN27G27G31BB27G29G31DJ2W82T731A129G31CG29G29G31CJ28831DW2752UY2UE27531B4311431D231C63109314J2NL2Y931AW31EA31DK2792MZ22U22N2VO2UH2Q22D52D5319Z31ET2RV31ES31EQ2P52SS2KF2V331EQ31BS2382DG2L42KF2D52DG29P31F52SS2D52PF2VD31EW2PJ2SS2MP2RO31F12PO31132TL2RO310K2W12ST31FB2382P92D531FE2VD31FH31EQ31CJ2MP31EE31A12KF2QE2SS2TL31G52SS2AN2QI2C331FA31FU2S12PT31FY2752TC2Q031EW31G323831GB310N2382QM31A131GA31132AN2QT31GF31F631GH2RV22F31EQ2R729P2QX2R12DG2782KF2UJ31GL23831FG31EY2D531FJ2YX31GR31AE31HL31GW2D22D52UB31H12SI31FX31A131GM2T631GO31A131G431132KF31GU31G931GQ31GX238319V31HP31H12L431HA23831H431GK31EQ311T31G12D522L31II23831EP31IC31IK2D52R727822G238311W31FZ31HG31HE31HI31HZ31FO31EC2KF31FM31BM31FR31HE31HR31IC22I31H531032RE2P331IR312J2EN31JF312Y2P32DG28131HC31HV31HF31GN31EQ31HJ2382MP21S31I1238313031EC2TL313A31FS31J831D131HU31FZ2Q631HH23831GP31HL2KF31HN313H31EC2AN31G531FS2AN31IB31D131GJ31JO31K72PY31HY31FK31I531J231GT31FP31KS31A12AN31I831H031KJ31HS28131IE31JO31IH31K831IK31K831IN313T28131IP31292P528131IT2YN31IW31JQ31IZ31KR31J431AE31LN31FQ2ZR31FT31KK2YO31JA31IQ31D131JD312931D1312E313T21W31JV28131JJ2YU314J2D52RX2SM310A2SV22U312Y2D5313X31EY281314431K8314631FN313X31FS31AQ2DG31AL2RV31LJ31HX31JR31J031JV31KT31JY2SW2PP31K02C3311W31HQ31H22A931K531HE31K731IY31K931J031KB31KW31I4314831KF31KW31KI31N723831KM22U31BD31G022C31KP31G231NE31JW31I331BM31HL31KY31LR31L131MR31ID31EQ31FZ31L631NC31L831NC31LA31AW31LD21W2P52A931IT22231JO31IX31EQ31LL2YX31LN31J331KV31J631EQ31K331AW31LV31LZ31AW31LY2R72A931M1312931JV2A931M623631M831AX31MB2EO31ME31EQ314A31EY2A931MK31NC31MM31GS314A31MP2RU2DG29G31JN31MU31IL31JS31JU31JW31N02RN31FT31K131N531LS31HS29G31N931EQ31NB31OL31ND31KR31NF31KD2HU31GC31NK31HE31O231E731NN31O531NQ31KO31Q631KA31NW31KV31NZ31I731O131H229G31L431O631LK23831O931Q631OB29G31OD2P529G31IT314J31PQ31K831PS31J131G631RA31I431OR31N631LT29G31OV2R729G31OY31QG312E2E431M32ZD31P531P72VM2SO31MC2SR2812D5315131MV29G31PG31Q631PI31AE31RZ31H031AQ31NP31EQ2UO22U2VC2MP315B31FS2T131FZ2U931K831EV31EQ2YC31NC2U731K82Z031FN21O31LR31F531K821P2QW2QP2D522O2392OJ2742ZC31T12SM2TL31EB314331NU29H31EQ2RX2ZC23631T231HE31AB275');local a=(bit or bit32);local d=a and a.bxor or function(a,b)local c,d,e=1,0,10 while a>0 and b>0 do local e,f=a%2,b%2 if e~=f then d=d+c end a,b,c=(a-e)/2,(b-f)/2,c*2 end if a<b then a=b end while a>0 do local b=a%2 if b>0 then d=d+c end a,c=(a-b)/2,c*2 end return d end local function c(b,a,c)if c then local a=(b/2^(a-1))%2^((c-1)-(a-1)+1);return a-a%1;else local a=2^(a-1);return(b%(a+a)>=a)and 1 or 0;end;end;local a=1;local function b()local b,f,c,e=h(j,a,a+3);b=d(b,116)f=d(f,116)c=d(c,116)e=d(e,116)a=a+4;return(e*16777216)+(c*65536)+(f*256)+b;end;local function i()local b=d(h(j,a,a),116);a=a+1;return b;end;local function f()local b,c=h(j,a,a+2);b=d(b,116)c=d(c,116)a=a+2;return(c*256)+b;end;local function q()local a=b();local b=b();local e=1;local d=(c(b,1,20)*(2^32))+a;local a=c(b,21,31);local b=((-1)^c(b,32));if(a==0)then if(d==0)then return b*0;else a=1;e=0;end;elseif(a==2047)then return(d==0)and(b*(1/0))or(b*(0/0));end;return n(b,a-1023)*(e+(d/(2^52)));end;local p=b;local function n(b)local c;if(not b)then b=p();if(b==0)then return'';end;end;c=e(j,a,a+b-1);a=a+b;local b={}for a=1,#c do b[a]=k(d(h(e(c,a,a)),116))end return m(b);end;local a=b;local function r(...)return{...},l('#',...)end local function m()local j={};local g={};local d={};local h={[#{{97;616;245;361};"1 + 1 = 111";}]=g,[#{{531;946;839;707};{771;305;953;45};"1 + 1 = 111";}]=nil,[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{392;448;630;827};}]=d,[#{"1 + 1 = 111";}]=j,};local a=b()local e={}for c=1,a do local b=i();local a;if(b==2)then a=(i()~=0);elseif(b==0)then a=q();elseif(b==3)then a=n();end;e[c]=a;end;for a=1,b()do g[a-1]=m();end;h[3]=i();for a=1,b()do d[a]=b();end;for h=1,b()do local a=i();if(c(a,1,1)==0)then local d=c(a,2,3);local g=c(a,4,6);local a={f(),f(),nil,nil};if(d==0)then a[#("Xds")]=f();a[#("vJza")]=f();elseif(d==1)then a[#("BpO")]=b();elseif(d==2)then a[#("Qsm")]=b()-(2^16)elseif(d==3)then a[#("omN")]=b()-(2^16)a[#("OX3S")]=f();end;if(c(g,1,1)==1)then a[#("Rh")]=e[a[#("2a")]]end if(c(g,2,2)==1)then a[#("N9V")]=e[a[#("X9B")]]end if(c(g,3,3)==1)then a[#("JJV1")]=e[a[#("yr1Y")]]end j[h]=a;end end;return h;end;local s=pcall local function n(k,i,f)k=(k==true and m())or k;return(function(...)local b=1;local h=-1;local j={...};local q=l('#',...)-1;local d=k[#{"1 + 1 = 111";}];local e=k[#{"1 + 1 = 111";{687;513;638;823};{475;1;468;65};}];local p=k[#{{484;737;739;414};"1 + 1 = 111";}];local function t()local l=r local k={};local m={};local c={};for a=0,q do if(a>=e)then k[a-e]=j[a+1];else c[a]=j[a+1];end;end;local a=q-e+1 local a;local e;while true do a=d[b];e=a[#("7")];if e<=#("Ttm9yTEiexzPeNngpPnEYgyX64jLOVWCMZDR")then if e<=#("r6Cfn1l2vMyPZZr3P")then if e<=#{"1 + 1 = 111";{641;638;588;549};"1 + 1 = 111";{396;896;857;327};"1 + 1 = 111";"1 + 1 = 111";{164;979;737;577};"1 + 1 = 111";}then if e<=#("L6d")then if e<=#("k")then if e>#("")then local b=a[#("dU")]c[b](g(c,b+1,a[#("8H2")]))else if(c[a[#("eP")]]==a[#("I48P")])then b=b+1;else b=a[#("fuZ")];end;end;elseif e>#("7T")then if(a[#{{390;506;357;851};"1 + 1 = 111";}]<=c[a[#("DJFp")]])then b=a[#("UYK")];else b=b+1;end;else c[a[#("c7")]]=f[a[#("rDC")]];end;elseif e<=#("yLom4")then if e>#("rW6Z")then local h;local e;f[a[#("RSZ")]]=c[a[#("Mt")]];b=b+1;a=d[b];c[a[#("lJ")]]=c[a[#("MQd")]][a[#("sj6W")]];b=b+1;a=d[b];e=a[#("c8")];h=c[a[#("LY5")]];c[e+1]=h;c[e]=h[a[#("5Dt1")]];b=b+1;a=d[b];c[a[#("NV")]]=f[a[#("oOE")]];b=b+1;a=d[b];e=a[#("lT")]c[e](g(c,e+1,a[#("MDs")]))else local e;c[a[#("e0")]][a[#("ykA")]]=a[#{{381;809;323;30};{980;772;77;266};{728;546;830;366};"1 + 1 = 111";}];b=b+1;a=d[b];c[a[#("B9")]]=f[a[#("EKT")]];b=b+1;a=d[b];c[a[#("KF")]]=c[a[#("Mtf")]][a[#("LZCS")]];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";"1 + 1 = 111";}]]=a[#("HbI")];b=b+1;a=d[b];c[a[#("SA")]]=a[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];b=b+1;a=d[b];c[a[#("J4")]]=a[#("Eq3")];b=b+1;a=d[b];e=a[#("4P")]c[e]=c[e](g(c,e+1,a[#("ANy")]))b=b+1;a=d[b];c[a[#("OF")]][a[#{"1 + 1 = 111";{610;555;968;319};{47;720;425;495};}]]=c[a[#("3PYY")]];b=b+1;a=d[b];c[a[#("tZ")]][a[#("jIv")]]=a[#("BKTE")];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";"1 + 1 = 111";}]][a[#("sFY")]]=a[#("esNk")];end;elseif e<=#("EI6VZV")then c[a[#("92")]]=c[a[#{{589;960;603;199};"1 + 1 = 111";{276;536;631;961};}]];elseif e>#("pD2mSJK")then local f;local e;e=a[#("HO")];f=c[a[#("TVP")]];c[e+1]=f;c[e]=f[a[#{"1 + 1 = 111";"1 + 1 = 111";{811;475;211;817};{563;404;61;904};}]];b=b+1;a=d[b];c[a[#("eM")]]=a[#("gzM")];b=b+1;a=d[b];e=a[#("Oc")]c[e]=c[e](g(c,e+1,a[#("pbA")]))b=b+1;a=d[b];c[a[#("GO")]]=c[a[#("ri5")]][a[#("489V")]];b=b+1;a=d[b];c[a[#("Qu")]]=c[a[#("lOf")]][a[#("C5BI")]];b=b+1;a=d[b];e=a[#("Be")];f=c[a[#("Npa")]];c[e+1]=f;c[e]=f[a[#("OhXE")]];b=b+1;a=d[b];e=a[#("Mr")]c[e](c[e+1])b=b+1;a=d[b];c[a[#{"1 + 1 = 111";"1 + 1 = 111";}]]=a[#("PbW")];b=b+1;a=d[b];i[a[#("tku")]]=c[a[#("th")]];else local e;c[a[#("Mb")]]=a[#("qMI")];b=b+1;a=d[b];e=a[#{{13;973;499;687};"1 + 1 = 111";}]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[#("2k")]]=f[a[#("7k9")]];b=b+1;a=d[b];c[a[#("2E")]]=c[a[#("kmJ")]][a[#("NuhG")]];b=b+1;a=d[b];c[a[#("pq")]]=a[#("hoo")];b=b+1;a=d[b];e=a[#("ei")]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[#("MN")]]=(a[#("J70")]~=0);b=b+1;a=d[b];c[a[#("Eh")]]=a[#("IkO")];end;elseif e<=#("rxnhq1JiqCyU")then if e<=#("BlY6QxgzhE")then if e>#("WySp2k2QM")then c[a[#("iy")]]=i[a[#("VPI")]];else local b=a[#("34")]local e={c[b](g(c,b+1,h))};local d=0;for a=b,a[#("vTZL")]do d=d+1;c[a]=e[d];end end;elseif e>#("t5IYIe5AQsC")then do return end;else c[a[#("gV")]]=a[#{"1 + 1 = 111";{260;407;22;857};"1 + 1 = 111";}];end;elseif e<=#{{28;564;958;25};{141;683;336;375};"1 + 1 = 111";{689;263;361;834};"1 + 1 = 111";{203;976;410;280};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{197;276;975;846};{151;676;691;309};"1 + 1 = 111";{16;842;416;418};}then if e==#("spfKSiFhpphir")then local b=a[#("Yc")];local d=c[a[#{{952;232;644;288};"1 + 1 = 111";{948;817;318;884};}]];c[b+1]=d;c[b]=d[a[#("UDYE")]];else if(c[a[#{{352;452;939;430};"1 + 1 = 111";}]]==a[#("70Iz")])then b=b+1;else b=a[#("Lr3")];end;end;elseif e<=#("8Bk2VR38X4ZDhCi")then c[a[#{"1 + 1 = 111";{634;731;655;349};}]]=(a[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]~=0);elseif e==#{{747;545;646;144};"1 + 1 = 111";"1 + 1 = 111";{773;191;792;701};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{768;432;185;667};{248;291;502;108};{307;417;780;979};"1 + 1 = 111";{194;732;415;718};{799;943;601;124};{394;44;927;800};"1 + 1 = 111";{881;192;997;682};}then local a=a[#("WI")]c[a](c[a+1])else local e;e=a[#("Hv")]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[#{"1 + 1 = 111";"1 + 1 = 111";}]]=f[a[#("R21")]];b=b+1;a=d[b];c[a[#("ES")]]=c[a[#("WMg")]][a[#("4Pdq")]];b=b+1;a=d[b];c[a[#("Qh")]]=a[#("tbq")];b=b+1;a=d[b];e=a[#("S2")]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[#("i9")]]=f[a[#{{324;197;684;935};{530;642;64;856};{480;203;851;374};}]];b=b+1;a=d[b];c[a[#("IV")]]=c[a[#("M4r")]][a[#("GjkJ")]];b=b+1;a=d[b];c[a[#("ZC")]]=a[#("bDC")];b=b+1;a=d[b];e=a[#("Nt")]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[#("Wz")]]=f[a[#("zJJ")]];end;elseif e<=#("sJTSaLlpuCkUoad9nJPEvJZ0Bi")then if e<=#("Gm68W5IY3ztP1CQqSz9F2")then if e<=#("SXpDBJUT2q1SQczEzZR")then if e==#("kK44YcQrgBCOazFiSt")then if(a[#("tS")]<=c[a[#("7GiG")]])then b=a[#("eZO")];else b=b+1;end;else local h;local e;c[a[#("VL")]]=a[#("HoW")];b=b+1;a=d[b];e=a[#{"1 + 1 = 111";"1 + 1 = 111";}]c[e](c[e+1])b=b+1;a=d[b];c[a[#("7N")]]=f[a[#("Yhr")]];b=b+1;a=d[b];c[a[#{{544;710;313;765};"1 + 1 = 111";}]]=c[a[#{{196;472;656;873};{894;50;103;363};{208;761;648;276};}]][a[#("eFDy")]];b=b+1;a=d[b];c[a[#("fb")]]=c[a[#("tVT")]][a[#("kizW")]];b=b+1;a=d[b];c[a[#("4d")]]=c[a[#("zLz")]][a[#("9g60")]];b=b+1;a=d[b];e=a[#("4o")];h=c[a[#("2zy")]];c[e+1]=h;c[e]=h[a[#("XJyN")]];b=b+1;a=d[b];c[a[#("2S")]]=a[#("Atc")];b=b+1;a=d[b];e=a[#("WX")]c[e]=c[e](g(c,e+1,a[#("dYq")]))b=b+1;a=d[b];c[a[#("MS")]]=c[a[#("x3J")]][a[#("7q0R")]];end;elseif e>#("9ejGcYiWN2nakYQ7h3vO")then local a=a[#("Pv")]c[a]=c[a](c[a+1])else local d=a[#("u7")]local e={c[d](g(c,d+1,h))};local b=0;for a=d,a[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{557;543;48;472};}]do b=b+1;c[a]=e[b];end end;elseif e<=#("3DMCZnSqIqWfuShbd2fPqcz")then if e>#("BrZtCxovPgfLHemLAFfMC5")then f[a[#("saE")]]=c[a[#("iI")]];else local d=a[#("3L")];local f=a[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{103;353;658;687};}];local e=d+2 local d={c[d](c[d+1],c[e])};for a=1,f do c[e+a]=d[a];end;local d=d[1]if d then c[e]=d b=a[#("MqA")];else b=b+1;end;end;elseif e<=#("gI6ebq9h0dTaIyzZkbABnMHE")then local e;local j;local k,n;local m;local e;c[a[#("PZ")]]=f[a[#("SXn")]];b=b+1;a=d[b];c[a[#("tH")]]=i[a[#("0c3")]];b=b+1;a=d[b];c[a[#("c2")]]=c[a[#("A4G")]][a[#("CykB")]];b=b+1;a=d[b];c[a[#("aA")]]=c[a[#("1ID")]][a[#("WqqE")]];b=b+1;a=d[b];e=a[#("V3")];m=c[a[#("fe7")]];c[e+1]=m;c[e]=m[a[#("zmuL")]];b=b+1;a=d[b];e=a[#("hY")]k,n=l(c[e](c[e+1]))h=n+e-1 j=0;for a=e,h do j=j+1;c[a]=k[j];end;b=b+1;a=d[b];e=a[#("ju")]k={c[e](g(c,e+1,h))};j=0;for a=e,a[#("yhGX")]do j=j+1;c[a]=k[j];end b=b+1;a=d[b];b=a[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];elseif e>#("PFoV7XCGCTWFsnfP8pIXePmbP")then local e;c[a[#("Uu")]][a[#("man")]]=a[#("XPVx")];b=b+1;a=d[b];c[a[#("FU")]]=f[a[#("g3h")]];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";{8;796;834;849};}]]=c[a[#("9kG")]][a[#("M2AV")]];b=b+1;a=d[b];c[a[#("sa")]]=a[#("fyx")];b=b+1;a=d[b];c[a[#("Pm")]]=a[#{{240;994;100;683};{908;91;804;50};{191;449;868;166};}];b=b+1;a=d[b];c[a[#("LC")]]=a[#("xA1")];b=b+1;a=d[b];e=a[#("5K")]c[e]=c[e](g(c,e+1,a[#("I9A")]))b=b+1;a=d[b];c[a[#("7O")]][a[#("tAO")]]=c[a[#("QZ3n")]];b=b+1;a=d[b];c[a[#("6K")]][a[#("GXC")]]=a[#("Az77")];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";{843;373;641;453};}]][a[#("YFx")]]=a[#("R9v2")];else local e;c[a[#("1U")]]=f[a[#("X4j")]];b=b+1;a=d[b];c[a[#("m4")]]=c[a[#("c0z")]][a[#("8oQj")]];b=b+1;a=d[b];c[a[#("FZ")]]=a[#("S7e")];b=b+1;a=d[b];e=a[#("nR")]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[#("ZS")]]=f[a[#("lZd")]];b=b+1;a=d[b];c[a[#("0f")]]=c[a[#("jD1")]][a[#("hYFK")]];b=b+1;a=d[b];c[a[#("9H")]]=a[#("EKr")];b=b+1;a=d[b];e=a[#("yn")]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[#("eX")]]=f[a[#("Heg")]];b=b+1;a=d[b];c[a[#("2I")]]=c[a[#("6Hm")]][a[#("XNXO")]];end;elseif e<=#("KbEMFbCfxVUx3prFfONt1XuVpx8R49r")then if e<=#("fbmAb0oUdn1t5MvrGJKIzudXRTvi")then if e>#{{365;310;414;441};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{336;823;14;281};{14;46;639;659};{13;190;785;840};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{49;533;399;843};"1 + 1 = 111";"1 + 1 = 111";{990;73;31;893};{672;52;59;343};{558;161;164;885};"1 + 1 = 111";{799;742;143;258};{211;846;270;711};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{267;78;325;658};{409;678;343;940};{320;55;723;389};}then c[a[#("a6")]]=c[a[#("AJP")]]+a[#{{680;666;189;678};{629;355;301;727};"1 + 1 = 111";{958;798;204;47};}];else c[a[#("VB")]]=c[a[#("qlS")]]+a[#("Ktgf")];end;elseif e<=#("ATsEgRscE0zuEpOguiGeA0Q2ShxKZ")then local a=a[#("xC")]c[a](c[a+1])elseif e==#("URG3NikVtl7LDkBsGBHoeLsQIKcAW8")then c[a[#("yg")]]=a[#("KT0")];else do return end;end;elseif e<=#("TnFfRZLMG6JZtgYxGCAM6cK3jzZudfU9u")then if e>#("oy7eUD5YbsFW8KTmH8xxyQNM6sapJAlK")then f[a[#("u3p")]]=c[a[#("FS")]];else local e;c[a[#("Ti")]]=c[a[#("UPQ")]][a[#("8jIZ")]];b=b+1;a=d[b];c[a[#("Gg")]]=a[#("Opc")];b=b+1;a=d[b];c[a[#("xz")]]=a[#("NKi")];b=b+1;a=d[b];c[a[#("zD")]]=a[#("ThU")];b=b+1;a=d[b];c[a[#("Gi")]]=a[#("UOu")];b=b+1;a=d[b];e=a[#("YN")]c[e]=c[e](g(c,e+1,a[#("jKF")]))b=b+1;a=d[b];c[a[#("Lm")]][a[#("VjH")]]=c[a[#("Xs2W")]];b=b+1;a=d[b];c[a[#("xe")]]=f[a[#("U5o")]];b=b+1;a=d[b];c[a[#("jD")]]=c[a[#("YAH")]][a[#("ymph")]];b=b+1;a=d[b];c[a[#("yL")]]=c[a[#("01W")]][a[#("2usy")]];end;elseif e<=#("D1BzBR6QhbryyAoL1IVM7EJUviBCQpLg5r")then c[a[#("S3")]]=(a[#("HCZ")]~=0);elseif e>#("TsXgqARpOunJ3WOS1B7G8sQdsqFa2BlDf3G")then local f;local e;c[a[#("1u")]]=c[a[#("cU8")]][a[#("WMs3")]];b=b+1;a=d[b];c[a[#("Tv")]]=a[#("9PM")];b=b+1;a=d[b];e=a[#("RO")]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[#("pv")]][a[#("IOH")]]=a[#{{53;412;6;379};"1 + 1 = 111";"1 + 1 = 111";{222;913;295;133};}];b=b+1;a=d[b];c[a[#("U0")]]=c[a[#("kSJ")]][a[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{42;448;631;851};}]];b=b+1;a=d[b];c[a[#("kK")]]=c[a[#("TrD")]][a[#("8pPY")]];b=b+1;a=d[b];c[a[#("v3")]][a[#("uFj")]]=c[a[#{"1 + 1 = 111";{995;516;480;148};{544;232;590;943};{422;941;555;215};}]];b=b+1;a=d[b];c[a[#("gx")]][a[#("KDt")]]=a[#("RLyH")];b=b+1;a=d[b];c[a[#{{598;64;717;61};"1 + 1 = 111";}]][a[#("1kf")]]=a[#("paTy")];b=b+1;a=d[b];e=a[#("08")];f=c[a[#("UX5")]];c[e+1]=f;c[e]=f[a[#("v0OV")]];else local h;local e;f[a[#{"1 + 1 = 111";{101;841;398;517};{582;635;142;126};}]]=c[a[#("eQ")]];b=b+1;a=d[b];c[a[#("bO")]]=c[a[#{"1 + 1 = 111";"1 + 1 = 111";{763;454;345;678};}]][a[#("t4hU")]];b=b+1;a=d[b];e=a[#("De")];h=c[a[#("3xg")]];c[e+1]=h;c[e]=h[a[#("qMFD")]];b=b+1;a=d[b];c[a[#("Y4")]]=f[a[#("rrB")]];b=b+1;a=d[b];e=a[#("ng")]c[e](g(c,e+1,a[#("8hx")]))b=b+1;a=d[b];c[a[#("sA")]][a[#("KP2")]]=c[a[#("MPFv")]];b=b+1;a=d[b];c[a[#("tn")]]=f[a[#("vSY")]];b=b+1;a=d[b];c[a[#{{455;180;344;210};"1 + 1 = 111";}]]=c[a[#("JZA")]][a[#("bMDn")]];b=b+1;a=d[b];c[a[#("9U")]]=a[#("XIt")];b=b+1;a=d[b];c[a[#("Ld")]]=a[#("Hzy")];end;elseif e<=#("dCEmqn4AiKIPcHTQ7VIAMUYa4QynjUD9quOA6VoUzq4SSZ8vRFGtvfQ")then if e<=#("ODsK0QpzgJzR2tTmGXbvZfseScHOnjNkPuVDCP4SaFMjB")then if e<=#("DyWtXJeuEJkn1YjLk65ocIIqU12suuDjOCJi24ve")then if e<=#{"1 + 1 = 111";{532;350;887;459};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{354;28;220;388};{95;301;856;196};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{494;372;75;503};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{738;264;653;251};{810;203;512;827};"1 + 1 = 111";"1 + 1 = 111";{239;887;575;206};{296;390;619;570};{861;973;479;68};{763;311;366;724};"1 + 1 = 111";{100;227;878;339};{196;686;440;100};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{259;223;590;860};{146;992;903;624};"1 + 1 = 111";"1 + 1 = 111";{606;131;970;674};"1 + 1 = 111";{229;140;945;585};{886;560;608;723};"1 + 1 = 111";{897;838;924;340};}then if e>#("eWU5aX5DmPsyuBytuQhqPx1IQdeycHlFHe03b")then local e;c[a[#("Z0")]][a[#("A8A")]]=a[#("of2D")];b=b+1;a=d[b];c[a[#("Ul")]]=f[a[#("xlM")]];b=b+1;a=d[b];c[a[#("yS")]]=c[a[#("U0T")]][a[#("Nymh")]];b=b+1;a=d[b];c[a[#("GS")]]=a[#("BzB")];b=b+1;a=d[b];c[a[#("mH")]]=a[#("knS")];b=b+1;a=d[b];c[a[#("73")]]=a[#("USM")];b=b+1;a=d[b];e=a[#("vy")]c[e]=c[e](g(c,e+1,a[#{{275;993;565;937};{719;696;704;757};"1 + 1 = 111";}]))b=b+1;a=d[b];c[a[#("aH")]][a[#("8VR")]]=c[a[#("hM42")]];b=b+1;a=d[b];c[a[#("Vh")]][a[#("TKg")]]=a[#("KNpR")];b=b+1;a=d[b];c[a[#("Kb")]][a[#("oPj")]]=a[#("ff5e")];else if(c[a[#("Y2")]]<=a[#("LGyk")])then b=b+1;else b=a[#("foN")];end;end;elseif e>#{"1 + 1 = 111";"1 + 1 = 111";{68;30;882;274};{446;875;38;907};"1 + 1 = 111";"1 + 1 = 111";{56;736;850;53};"1 + 1 = 111";{581;717;575;599};"1 + 1 = 111";"1 + 1 = 111";{430;805;148;97};"1 + 1 = 111";{964;51;765;665};"1 + 1 = 111";{111;146;420;301};{48;286;476;878};{23;990;84;498};{395;267;297;238};"1 + 1 = 111";"1 + 1 = 111";{675;911;911;52};{909;265;793;249};"1 + 1 = 111";"1 + 1 = 111";{339;718;989;351};"1 + 1 = 111";{809;217;443;297};{793;25;725;145};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{477;976;824;834};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}then local e;local i;local j,m;local k;local e;c[a[#{"1 + 1 = 111";{955;44;247;805};}]]=f[a[#("fX7")]];b=b+1;a=d[b];c[a[#{{567;89;2;391};"1 + 1 = 111";}]]=c[a[#("gYE")]][a[#("UyAz")]];b=b+1;a=d[b];c[a[#("c4")]]=c[a[#("QXb")]][a[#("nbO8")]];b=b+1;a=d[b];c[a[#("AX")]]=f[a[#("xxp")]];b=b+1;a=d[b];c[a[#("HU")]]=c[a[#("02L")]][a[#("2Ayj")]];b=b+1;a=d[b];e=a[#("bc")];k=c[a[#("jj3")]];c[e+1]=k;c[e]=k[a[#("aUNN")]];b=b+1;a=d[b];e=a[#("To")]j,m=l(c[e](c[e+1]))h=m+e-1 i=0;for a=e,h do i=i+1;c[a]=j[i];end;b=b+1;a=d[b];e=a[#("cY")]j={c[e](g(c,e+1,h))};i=0;for a=e,a[#("zvWY")]do i=i+1;c[a]=j[i];end b=b+1;a=d[b];b=a[#("rZq")];else local e=a[#("39")];local f=a[#("jkXY")];local d=e+2 local e={c[e](c[e+1],c[d])};for a=1,f do c[d+a]=e[a];end;local e=e[1]if e then c[d]=e b=a[#("dIF")];else b=b+1;end;end;elseif e<=#("0vh45mjjrZoi8ZYmJIQHg4FQK7HfFyGqIOv3ZYMnHs")then if e==#("abBGDDtqN2Nk51Bt7PdP4t7KuD4yU5C9XzEPjCeNl")then b=a[#("f47")];else c[a[#{"1 + 1 = 111";{405;816;64;654};}]][a[#("V7N")]]=c[a[#("habH")]];end;elseif e<=#("3y5DBczEPIDOLRd0l9I5GRBNyHxVkGKBDXAJP2c29qq")then local h;local e;c[a[#("sS")]]=f[a[#("qy3")]];b=b+1;a=d[b];c[a[#("D5")]]=c[a[#("Jzo")]][a[#("UlFk")]];b=b+1;a=d[b];c[a[#("4d")]]=c[a[#("zGt")]][a[#("J8rk")]];b=b+1;a=d[b];e=a[#("tt")];h=c[a[#("ONJ")]];c[e+1]=h;c[e]=h[a[#("PSVU")]];b=b+1;a=d[b];c[a[#("pL")]]=a[#("4hg")];b=b+1;a=d[b];e=a[#("po")]c[e]=c[e](g(c,e+1,a[#("H8p")]))b=b+1;a=d[b];c[a[#("FJ")]][a[#("rGN")]]=c[a[#("03UH")]];b=b+1;a=d[b];c[a[#("cf")]][a[#("zf3")]]=c[a[#("zLLh")]];b=b+1;a=d[b];c[a[#("xn")]]=f[a[#("pBS")]];b=b+1;a=d[b];c[a[#("Va")]]=c[a[#("q6r")]][a[#("dn0X")]];b=b+1;a=d[b];c[a[#("1R")]]=a[#("Lyg")];b=b+1;a=d[b];c[a[#("9h")]]=a[#("nr1")];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";{2;659;590;570};}]]=a[#("ubp")];b=b+1;a=d[b];e=a[#("qg")]c[e]=c[e](g(c,e+1,a[#("1vN")]))b=b+1;a=d[b];c[a[#("Cz")]][a[#("iVP")]]=c[a[#("2y0M")]];b=b+1;a=d[b];c[a[#("lW")]]=f[a[#{{642;742;289;273};{826;439;614;953};"1 + 1 = 111";}]];b=b+1;a=d[b];c[a[#("JN")]]=c[a[#("MB8")]][a[#("YoCi")]];b=b+1;a=d[b];c[a[#("Q0")]]=a[#("5XQ")];b=b+1;a=d[b];c[a[#("Sp")]]=a[#("0mQ")];b=b+1;a=d[b];c[a[#("mg")]]=a[#("2R3")];b=b+1;a=d[b];c[a[#("xi")]]=a[#("Plh")];b=b+1;a=d[b];e=a[#{{243;408;371;308};"1 + 1 = 111";}]c[e]=c[e](g(c,e+1,a[#("0pb")]))b=b+1;a=d[b];c[a[#("xq")]][a[#("XBN")]]=c[a[#{"1 + 1 = 111";{594;253;67;556};"1 + 1 = 111";"1 + 1 = 111";}]];b=b+1;a=d[b];c[a[#("OL")]]=f[a[#("qoh")]];b=b+1;a=d[b];c[a[#("Jo")]]=c[a[#("4X5")]][a[#("Bzdj")]];b=b+1;a=d[b];c[a[#("9K")]]=a[#("tOH")];b=b+1;a=d[b];c[a[#("Tk")]]=a[#("vrX")];b=b+1;a=d[b];c[a[#("7l")]]=a[#("QEz")];b=b+1;a=d[b];c[a[#("Tk")]]=a[#("1Qx")];b=b+1;a=d[b];e=a[#("2r")]c[e]=c[e](g(c,e+1,a[#("OgD")]))b=b+1;a=d[b];c[a[#("DD")]][a[#("zeA")]]=c[a[#("opFt")]];b=b+1;a=d[b];c[a[#("g3")]][a[#("jkR")]]=a[#("iKyN")];b=b+1;a=d[b];c[a[#("6G")]][a[#("f1o")]]=c[a[#("uiFW")]];b=b+1;a=d[b];c[a[#("rZ")]]=f[a[#{{14;924;401;880};{841;268;319;839};{361;590;686;603};}]];b=b+1;a=d[b];c[a[#("U5")]]=c[a[#{"1 + 1 = 111";"1 + 1 = 111";{787;258;697;72};}]][a[#("r1jk")]];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";"1 + 1 = 111";}]]=a[#("Dym")];b=b+1;a=d[b];c[a[#("WS")]]=a[#("cmN")];b=b+1;a=d[b];c[a[#("6D")]]=a[#("1Gk")];b=b+1;a=d[b];e=a[#("pA")]c[e]=c[e](g(c,e+1,a[#("tKy")]))b=b+1;a=d[b];c[a[#("Qm")]][a[#("ncz")]]=c[a[#("LBMD")]];b=b+1;a=d[b];c[a[#("VE")]]=f[a[#("KmI")]];b=b+1;a=d[b];c[a[#("Mk")]]=c[a[#("psP")]][a[#("u9tG")]];b=b+1;a=d[b];c[a[#("oD")]]=a[#("ax6")];b=b+1;a=d[b];c[a[#("Ed")]]=a[#{{601;520;84;882};{132;141;165;572};{158;940;504;117};}];b=b+1;a=d[b];c[a[#{{276;488;81;680};"1 + 1 = 111";}]]=a[#{{885;580;866;863};{902;576;514;202};"1 + 1 = 111";}];b=b+1;a=d[b];c[a[#("5m")]]=a[#("HhT")];b=b+1;a=d[b];e=a[#("uj")]c[e]=c[e](g(c,e+1,a[#("RBW")]))b=b+1;a=d[b];c[a[#{"1 + 1 = 111";{48;655;104;9};}]][a[#("TBW")]]=c[a[#{"1 + 1 = 111";"1 + 1 = 111";{943;54;933;514};"1 + 1 = 111";}]];b=b+1;a=d[b];c[a[#("lH")]]=f[a[#("kZ8")]];b=b+1;a=d[b];c[a[#("a0")]]=c[a[#("0ze")]][a[#("M3HD")]];b=b+1;a=d[b];c[a[#("bq")]]=c[a[#("H2J")]][a[#("n1YS")]];b=b+1;a=d[b];c[a[#("OG")]][a[#("KfS")]]=c[a[#("rJZN")]];b=b+1;a=d[b];c[a[#("Ii")]][a[#("Qxx")]]=a[#("Kp3s")];b=b+1;a=d[b];c[a[#("4u")]]=f[a[#("LCO")]];b=b+1;a=d[b];c[a[#("qr")]]=c[a[#("E8h")]][a[#("XObI")]];b=b+1;a=d[b];c[a[#("Mm")]]=a[#("HEb")];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";"1 + 1 = 111";}]]=a[#("Kt4")];b=b+1;a=d[b];c[a[#("Qv")]]=a[#("6Nk")];b=b+1;a=d[b];e=a[#{"1 + 1 = 111";"1 + 1 = 111";}]c[e]=c[e](g(c,e+1,a[#("cTA")]))b=b+1;a=d[b];c[a[#("zA")]][a[#("In9")]]=c[a[#("jq2H")]];b=b+1;a=d[b];c[a[#("in")]][a[#("TyF")]]=a[#("kCdM")];b=b+1;a=d[b];c[a[#("0D")]][a[#("dPb")]]=a[#{"1 + 1 = 111";"1 + 1 = 111";{971;89;562;932};{525;138;576;951};}];b=b+1;a=d[b];c[a[#("Uf")]][a[#("lFW")]]=a[#("UM3U")];b=b+1;a=d[b];c[a[#("by")]][a[#("qpm")]]=c[a[#("WkQl")]];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";"1 + 1 = 111";}]]=f[a[#{{689;965;13;791};{425;332;236;709};{467;935;31;517};}]];b=b+1;a=d[b];c[a[#("z9")]]=c[a[#("kCC")]][a[#("AqxR")]];b=b+1;a=d[b];c[a[#("4K")]]=a[#{"1 + 1 = 111";{797;496;133;91};{127;447;651;218};}];b=b+1;a=d[b];c[a[#("7B")]]=a[#("b95")];b=b+1;a=d[b];c[a[#("ru")]]=a[#("9Gf")];b=b+1;a=d[b];e=a[#("rz")]c[e]=c[e](g(c,e+1,a[#("8QH")]))b=b+1;a=d[b];c[a[#{{306;873;905;264};"1 + 1 = 111";}]][a[#("ske")]]=c[a[#("718O")]];b=b+1;a=d[b];c[a[#("gV")]]=f[a[#("0sm")]];b=b+1;a=d[b];c[a[#("bA")]]=c[a[#("HxX")]][a[#("79r6")]];b=b+1;a=d[b];c[a[#("21")]]=a[#("sTB")];b=b+1;a=d[b];c[a[#("hI")]]=a[#("5Bk")];b=b+1;a=d[b];c[a[#("ik")]]=a[#("JjR")];b=b+1;a=d[b];c[a[#("m0")]]=a[#("KH2")];b=b+1;a=d[b];e=a[#("JF")]c[e]=c[e](g(c,e+1,a[#("kde")]))b=b+1;a=d[b];c[a[#("ul")]][a[#("Ca6")]]=c[a[#("0GnK")]];b=b+1;a=d[b];c[a[#("gI")]]=f[a[#("xan")]];elseif e==#("HiXWLsqfepLl7se3PNtj8clXqFls6Q6pAHgoTLk1oFxm")then local b=a[#("2C")]c[b]=c[b](g(c,b+1,a[#("Rtu")]))else local e;e=a[#("3e")]c[e]=c[e](g(c,e+1,a[#("mx7")]))b=b+1;a=d[b];c[a[#("uA")]][a[#("fYm")]]=c[a[#("pIkR")]];b=b+1;a=d[b];c[a[#("Sy")]]=f[a[#("Gxv")]];b=b+1;a=d[b];c[a[#("9c")]]=c[a[#("E21")]][a[#{"1 + 1 = 111";{445;195;582;391};"1 + 1 = 111";{649;385;762;485};}]];b=b+1;a=d[b];c[a[#("mZ")]]=a[#("BCM")];b=b+1;a=d[b];c[a[#("Jj")]]=a[#("rMg")];b=b+1;a=d[b];c[a[#("af")]]=a[#("WB4")];b=b+1;a=d[b];c[a[#("Fx")]]=a[#("nrD")];b=b+1;a=d[b];e=a[#("3W")]c[e]=c[e](g(c,e+1,a[#("Yc9")]))b=b+1;a=d[b];c[a[#("t4")]][a[#("JNP")]]=c[a[#{{64;186;410;223};"1 + 1 = 111";{664;900;602;653};{303;612;884;327};}]];end;elseif e<=#("oMxXimv6h5E79Fgh7jysvVAlZkeDD4DQ8Lc3ZFXELtsLMrTfdU")then if e<=#("u831Dlk88h3DmCY8zDnrCv4ScDZKIB9zTNhReUKROHZxR0f")then if e==#("XtuN0CY9ekZ9vLBIiFUJth3P2GO5GIblxQWofvIrYiN34K")then local e;e=a[#("Ra")]c[e]=c[e](g(c,e+1,a[#("0HP")]))b=b+1;a=d[b];c[a[#("An")]][a[#{"1 + 1 = 111";{501;944;480;155};"1 + 1 = 111";}]]=c[a[#("3fvp")]];b=b+1;a=d[b];c[a[#("SX")]]=f[a[#("i4C")]];b=b+1;a=d[b];c[a[#("oE")]]=c[a[#("R2y")]][a[#{"1 + 1 = 111";"1 + 1 = 111";{993;338;566;630};"1 + 1 = 111";}]];b=b+1;a=d[b];c[a[#("7K")]]=a[#("qPD")];b=b+1;a=d[b];c[a[#("hh")]]=a[#("3rt")];b=b+1;a=d[b];c[a[#("4I")]]=a[#("4gu")];b=b+1;a=d[b];c[a[#("71")]]=a[#("3OT")];b=b+1;a=d[b];e=a[#("iz")]c[e]=c[e](g(c,e+1,a[#("XoN")]))b=b+1;a=d[b];c[a[#("LC")]][a[#("7bO")]]=c[a[#("Vu6l")]];else c[a[#("gy")]]();end;elseif e<=#("dgrnmfHYQAQUuX3DGjNNQZmCW6DVlEaUrkLYotYf01gYAMnE")then local a=a[#("Rr")]c[a]=c[a](c[a+1])elseif e==#("PgUr7Pn4ZCqNWNlA6CjmfnmuHXZTyckS90GxpCuGx3A2IDen4")then c[a[#{"1 + 1 = 111";{769;906;569;451};}]][a[#("4AX")]]=a[#("q6go")];else c[a[#("z1")]]=i[a[#("ZnI")]];end;elseif e<=#("EjeqZB4zUkZFHXrIO5gZjEhO0mYuWeSLZ8IaOSaeC1SjQ1vMKaYi")then if e>#("epacABNNKMQCoQJoq454bxrW7880mUWpKEUSI8nryC2obSBlXxs")then c[a[#("AV")]][a[#("Pz7")]]=a[#("1gQR")];else local h;local e;f[a[#("j9D")]]=c[a[#("gI")]];b=b+1;a=d[b];c[a[#("lW")]]=c[a[#("nBk")]][a[#("mJ4N")]];b=b+1;a=d[b];e=a[#("nA")];h=c[a[#("CfL")]];c[e+1]=h;c[e]=h[a[#("xrqL")]];b=b+1;a=d[b];c[a[#("CU")]]=f[a[#("kOC")]];b=b+1;a=d[b];e=a[#("bq")]c[e](g(c,e+1,a[#("oNM")]))b=b+1;a=d[b];c[a[#("Wh")]][a[#("bEV")]]=c[a[#("Vj8F")]];b=b+1;a=d[b];c[a[#("gi")]]=f[a[#("E9y")]];b=b+1;a=d[b];c[a[#{{784;119;921;462};"1 + 1 = 111";}]]=c[a[#("JzW")]][a[#("3GTb")]];b=b+1;a=d[b];c[a[#("AX")]]=a[#("RZO")];b=b+1;a=d[b];c[a[#("UG")]]=a[#("WeG")];end;elseif e<=#{{816;233;242;614};"1 + 1 = 111";{324;116;998;997};{75;781;631;906};{517;387;362;267};"1 + 1 = 111";{806;377;440;176};"1 + 1 = 111";"1 + 1 = 111";{541;985;85;570};"1 + 1 = 111";{151;296;51;413};{21;186;445;67};"1 + 1 = 111";{695;714;716;704};{444;358;556;162};{660;199;688;373};{363;194;41;105};{319;200;38;329};"1 + 1 = 111";{528;189;780;564};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{471;145;132;848};{200;531;586;527};"1 + 1 = 111";"1 + 1 = 111";{751;27;446;756};{205;746;176;858};{731;542;503;313};"1 + 1 = 111";{100;98;176;332};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{252;203;955;751};{847;913;573;969};"1 + 1 = 111";{200;56;94;21};{870;980;862;424};{763;741;688;119};"1 + 1 = 111";{115;881;102;721};{866;452;246;694};"1 + 1 = 111";"1 + 1 = 111";{892;990;782;680};{960;720;430;896};"1 + 1 = 111";{825;626;552;356};{151;431;858;106};}then if(c[a[#("dH")]]~=a[#("0YgA")])then b=b+1;else b=a[#("0gH")];end;elseif e==#("zpRHn4EZ5PULzjdFy4fxA5X4HCOiz1IfjBrgQ1Y00d0l2COpHvsu1t")then c[a[#{{382;819;636;763};{711;832;872;441};}]]=f[a[#("Ytj")]];else local a=a[#("4z")]local d,b=l(c[a](c[a+1]))h=b+a-1 local b=0;for a=a,h do b=b+1;c[a]=d[b];end;end;elseif e<=#("DCW9VquBdgOB717ZHgpHveMcfYzLdInnZ1YO31cKFNWenaQyKGWoMXny0T471UyF")then if e<=#("BLgcs5PdQbTrHZeiabHW9LcNAYk6fSVoqmWzKvrLgk6VEfs3ZY1S1T30JDM")then if e<=#("VT77qFbudQIPU5QYOrjtFqgq0cyIt50hTXZxm8E9e80jqm85celqtr8FM")then if e==#("hogDbh0B56fsMPYjpHA7aOdDFoUJXBYuVH1o3M6Tt0qbZUDHDjcCePQE")then c[a[#("93")]]=c[a[#("WfR")]][a[#("cECU")]];else c[a[#("ho")]][a[#{{500;445;389;63};{794;700;88;449};{188;664;395;630};}]]=c[a[#("XzPe")]];end;elseif e>#("O7WyqNEiVIeYJqNKRNkxbNVWmfOzxpf0ydpOkucmX3dlyS43z1ybGgjala")then c[a[#("3r")]]=c[a[#("o8e")]];else local h;local e;c[a[#("WM")]]=f[a[#("cE8")]];b=b+1;a=d[b];e=a[#("at")];h=c[a[#{"1 + 1 = 111";{83;216;309;1};{428;711;691;223};}]];c[e+1]=h;c[e]=h[a[#("8BAh")]];b=b+1;a=d[b];c[a[#("Fh")]]=a[#("9OQ")];b=b+1;a=d[b];e=a[#("FV")]c[e]=c[e](g(c,e+1,a[#("ggy")]))b=b+1;a=d[b];c[a[#("tD")]]=c[a[#("65P")]][a[#("DevH")]];b=b+1;a=d[b];c[a[#("Pz")]]=c[a[#("0m3")]][a[#("g8M0")]];b=b+1;a=d[b];e=a[#("co")];h=c[a[#("RUR")]];c[e+1]=h;c[e]=h[a[#("vxPC")]];b=b+1;a=d[b];c[a[#("82")]]=c[a[#("68I")]];b=b+1;a=d[b];e=a[#("Pg")]c[e](g(c,e+1,a[#("9rE")]))b=b+1;a=d[b];c[a[#("h1")]]=(a[#("iEG")]~=0);b=b+1;a=d[b];i[a[#("HYl")]]=c[a[#{{451;428;935;842};"1 + 1 = 111";}]];b=b+1;a=d[b];c[a[#("Y7")]]=f[a[#("zH4")]];b=b+1;a=d[b];c[a[#("7d")]]=a[#("t8T")];b=b+1;a=d[b];e=a[#("Dr")]c[e](c[e+1])b=b+1;a=d[b];c[a[#("Jz")]]=f[a[#("s4z")]];b=b+1;a=d[b];c[a[#("SP")]]=c[a[#("LFv")]][a[#("zCF1")]];b=b+1;a=d[b];c[a[#("eD")]]=c[a[#("zXy")]][a[#("30Gh")]];b=b+1;a=d[b];c[a[#("t1")]]=c[a[#{{772;784;274;541};{885;478;298;828};"1 + 1 = 111";}]][a[#("vF4M")]];b=b+1;a=d[b];e=a[#{"1 + 1 = 111";{869;239;564;321};}];h=c[a[#("MbV")]];c[e+1]=h;c[e]=h[a[#("CfMT")]];b=b+1;a=d[b];c[a[#("bu")]]=a[#("z7N")];b=b+1;a=d[b];e=a[#("yx")]c[e]=c[e](g(c,e+1,a[#{{782;993;191;42};{6;407;514;155};{489;956;771;477};}]))b=b+1;a=d[b];if(c[a[#("rV")]]~=a[#("WDKH")])then b=b+1;else b=a[#("0bP")];end;end;elseif e<=#("k9fWGCoBGb8AvL7KiKJzFlU9F1duq3oCkk1nRgITiry2BBcBIHbBNLQ8ofqOz")then if e==#("jMWGpkTT2bbZpmX1JdZNWU1YZJF38LZ4uohWg4l1SYO9zXvDkxHmZViAV7RQ")then local a=a[#("DG")]local d,b=l(c[a](c[a+1]))h=b+a-1 local b=0;for a=a,h do b=b+1;c[a]=d[b];end;else local b=a[#("aR")]c[b]=c[b](g(c,b+1,a[#("poE")]))end;elseif e<=#("0VqlhFbebVO2747f2zcnbSLeNfJfRbinFk2dxXrrtzjL3u11lu2JODPhjmJc55")then local e;c[a[#("aJ")]]=c[a[#{{207;761;871;988};"1 + 1 = 111";{774;829;893;182};}]][a[#("d1Lx")]];b=b+1;a=d[b];c[a[#("tz")]]=a[#("i8s")];b=b+1;a=d[b];c[a[#("e7")]]=a[#("Akc")];b=b+1;a=d[b];c[a[#("Yd")]]=a[#("vfd")];b=b+1;a=d[b];c[a[#("jA")]]=a[#("mp4")];b=b+1;a=d[b];e=a[#("DI")]c[e]=c[e](g(c,e+1,a[#("ryZ")]))b=b+1;a=d[b];c[a[#("j6")]][a[#("AkS")]]=c[a[#("AUmT")]];b=b+1;a=d[b];c[a[#("9e")]]=f[a[#("hBW")]];b=b+1;a=d[b];c[a[#("Pq")]]=c[a[#("zf6")]][a[#("G6I1")]];b=b+1;a=d[b];c[a[#("yo")]]=c[a[#("qit")]][a[#("MInP")]];elseif e==#("aNBxXc3SehU3MJ9krnS4xiKJcGU4kopxzbi8D7eYrMYC3JcJjbqYmaa2d1uqs9I")then if(c[a[#("4d")]]<=a[#("Me9B")])then b=b+1;else b=a[#("P2L")];end;else local h=p[a[#("SJY")]];local g;local e={};g=o({},{__index=function(b,a)local a=e[a];return a[1][a[2]];end,__newindex=function(c,a,b)local a=e[a]a[1][a[2]]=b;end;});for f=1,a[#("pV5Q")]do b=b+1;local a=d[b];if a[#("m")]==6 then e[f-1]={c,a[#("7xU")]};else e[f-1]={i,a[#("uiX")]};end;m[#m+1]=e;end;c[a[#("Gs")]]=n(h,g,f);end;elseif e<=#("1yFLAbSuj4NUtiPDDkUi7Cjybp4LMXGre8KGeCjis6OsypJ5l2Yhpz2AnhKjhgSxzuQuI")then if e<=#("ybbM0aX19WR8AU9ycQgks719blor4dJnycEWgOJ1MxhYCiR7yaraoy0BjbKOWG66mE")then if e>#("ypmqzgoI5ZdH3Fq43VJ89lcMed4egAlL8HsSkT33905MgFRiGLdkNFMmnKmumkBGN")then local b=a[#("f6")]c[b](g(c,b+1,a[#("Y5n")]))else local h=p[a[#("q5N")]];local g;local e={};g=o({},{__index=function(b,a)local a=e[a];return a[1][a[2]];end,__newindex=function(c,a,b)local a=e[a]a[1][a[2]]=b;end;});for f=1,a[#("527m")]do b=b+1;local a=d[b];if a[#("n")]==6 then e[f-1]={c,a[#("ymg")]};else e[f-1]={i,a[#("ieb")]};end;m[#m+1]=e;end;c[a[#("q6")]]=n(h,g,f);end;elseif e<=#("JvmITj1Q8ipBGKvWIGxa8D4fFLHIRZAA8O5v6823t7GD6WeM9BM5iNEfBgdiMt8iT0C")then local e;c[a[#("WK")]]=c[a[#{{800;740;740;911};"1 + 1 = 111";{841;121;593;863};}]][a[#("bpj8")]];b=b+1;a=d[b];c[a[#("0h")]]=a[#("W8i")];b=b+1;a=d[b];c[a[#("Ka")]]=a[#("x7B")];b=b+1;a=d[b];c[a[#("x1")]]=a[#("QXF")];b=b+1;a=d[b];c[a[#("Mb")]]=a[#("rBk")];b=b+1;a=d[b];e=a[#("cO")]c[e]=c[e](g(c,e+1,a[#("5vk")]))b=b+1;a=d[b];c[a[#("ZR")]][a[#("pLC")]]=c[a[#("Lrki")]];b=b+1;a=d[b];c[a[#("q3")]]=f[a[#("CHM")]];b=b+1;a=d[b];c[a[#{"1 + 1 = 111";"1 + 1 = 111";}]]=c[a[#("vQd")]][a[#("FIVu")]];b=b+1;a=d[b];c[a[#("xx")]]=c[a[#("CzT")]][a[#("oo49")]];elseif e>#("OaZKNDRa7CiSG5JqnFqvk0404Tr98xTgtm79LbrQ6Di97vMRVS5oKgRYg9Q4lRcKScyt")then i[a[#("WvL")]]=c[a[#("U2")]];else b=a[#("E2t")];end;elseif e<=#("JPlnKzRS42IhKoqCFGnFj2MvyFoBIr58rUlcTbaR9flghWLDVhmGkZXRc00ekqjN7KZ0cnT")then if e==#("GGGeQGnL3VPBezXD6Fa2l5HS5JiI6VAIzT9OsTaHMokzMTIJWx3In0sL9XihxQOivgbvzi")then i[a[#("R19")]]=c[a[#("vn")]];else local b=a[#("LZ")];local d=c[a[#("3Qj")]];c[b+1]=d;c[b]=d[a[#{{234;758;641;142};{184;973;241;148};"1 + 1 = 111";"1 + 1 = 111";}]];end;elseif e<=#("mFDq6UhgmbKVK11uJAzPGL2j6LcdFRljNmRdUKx11Q5fX4dqEWD6aENMMstvSeLFZAhykYK9")then c[a[#("sY")]]=c[a[#("s7i")]][a[#("OZHl")]];elseif e>#{"1 + 1 = 111";{626;271;418;242};{783;901;627;737};"1 + 1 = 111";{831;594;909;708};"1 + 1 = 111";{872;75;955;990};"1 + 1 = 111";{642;43;928;344};"1 + 1 = 111";{859;287;873;785};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{980;830;57;476};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{492;29;291;417};"1 + 1 = 111";{540;868;188;337};{993;14;966;769};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{493;135;180;106};{867;189;763;746};{817;734;73;340};{995;849;397;846};"1 + 1 = 111";"1 + 1 = 111";{287;496;290;716};"1 + 1 = 111";{730;550;304;366};{805;594;901;577};{932;244;842;875};{563;300;441;861};{322;800;762;289};"1 + 1 = 111";{553;700;519;89};{470;53;456;873};"1 + 1 = 111";{917;386;13;490};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{760;329;709;530};{685;893;772;47};{12;541;765;7};"1 + 1 = 111";"1 + 1 = 111";{903;588;180;351};{897;856;193;969};"1 + 1 = 111";{414;213;69;452};{15;209;708;810};"1 + 1 = 111";"1 + 1 = 111";{781;757;13;279};"1 + 1 = 111";{774;890;420;949};"1 + 1 = 111";{605;371;390;987};"1 + 1 = 111";{571;840;761;863};"1 + 1 = 111";{586;694;166;450};"1 + 1 = 111";{491;802;14;91};"1 + 1 = 111";"1 + 1 = 111";}then if(c[a[#("lI")]]~=a[#("O8vO")])then b=b+1;else b=a[#("HNA")];end;else c[a[#("a4")]]();end;b=b+1;end;end;A,B=r(s(t))if not A[1]then local a=k[4][b]or'?';error('ERROR IN IRONBREW SCRIPT [LINE '..a..']:'..A[2]);wait(9e9);else return g(A,2,B);end;end);end;return n(true,{},t())();end)(string.byte,table.insert,setmetatable);