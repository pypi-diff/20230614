# Comparing `tmp/publicsuffixlist-0.9.3.tar.gz` & `tmp/publicsuffixlist-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publicsuffixlist-0.9.3.tar", last modified: Tue Jan 31 06:13:08 2023, max compression
+gzip compressed data, was "publicsuffixlist-0.9.4.tar", last modified: Sat Apr 15 13:38:37 2023, max compression
```

## Comparing `publicsuffixlist-0.9.3.tar` & `publicsuffixlist-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 cause     (1000) cause     (1000)        0 2023-01-31 06:13:08.513105 publicsuffixlist-0.9.3/
--rw-rw-r--   0 cause     (1000) cause     (1000)    15922 2014-11-20 12:19:18.000000 publicsuffixlist-0.9.3/LICENSE
--rw-rw-r--   0 cause     (1000) cause     (1000)       36 2015-09-22 17:58:20.000000 publicsuffixlist-0.9.3/MANIFEST.in
--rw-rw-r--   0 cause     (1000) cause     (1000)     4394 2023-01-31 06:13:08.513105 publicsuffixlist-0.9.3/PKG-INFO
--rw-rw-r--   0 cause     (1000) cause     (1000)     3782 2022-06-03 13:28:42.000000 publicsuffixlist-0.9.3/README.md
-drwxrwxr-x   0 cause     (1000) cause     (1000)        0 2023-01-31 06:13:08.509106 publicsuffixlist-0.9.3/publicsuffixlist/
--rw-rw-r--   0 cause     (1000) cause     (1000)     8433 2022-09-28 05:59:35.000000 publicsuffixlist-0.9.3/publicsuffixlist/__init__.py
--rw-rw-r--   0 cause     (1000) cause     (1000)      917 2020-05-26 11:13:30.000000 publicsuffixlist-0.9.3/publicsuffixlist/compat.py
--rw-rw-r--   0 cause     (1000) cause     (1000)   244920 2023-01-31 06:12:56.000000 publicsuffixlist-0.9.3/publicsuffixlist/public_suffix_list.dat
--rw-rw-r--   0 cause     (1000) cause     (1000)    10884 2022-09-28 05:59:35.000000 publicsuffixlist-0.9.3/publicsuffixlist/test.py
--rw-rw-r--   0 cause     (1000) cause     (1000)     4308 2021-12-16 03:54:52.000000 publicsuffixlist-0.9.3/publicsuffixlist/test_psl.txt
--rw-rw-r--   0 cause     (1000) cause     (1000)     1662 2023-01-31 06:12:56.000000 publicsuffixlist-0.9.3/publicsuffixlist/update.py
-drwxrwxr-x   0 cause     (1000) cause     (1000)        0 2023-01-31 06:13:08.509106 publicsuffixlist-0.9.3/publicsuffixlist.egg-info/
--rw-rw-r--   0 cause     (1000) cause     (1000)     4394 2023-01-31 06:13:08.000000 publicsuffixlist-0.9.3/publicsuffixlist.egg-info/PKG-INFO
--rw-rw-r--   0 cause     (1000) cause     (1000)      503 2023-01-31 06:13:08.000000 publicsuffixlist-0.9.3/publicsuffixlist.egg-info/SOURCES.txt
--rw-rw-r--   0 cause     (1000) cause     (1000)        1 2023-01-31 06:13:08.000000 publicsuffixlist-0.9.3/publicsuffixlist.egg-info/dependency_links.txt
--rw-rw-r--   0 cause     (1000) cause     (1000)       80 2023-01-31 06:13:08.000000 publicsuffixlist-0.9.3/publicsuffixlist.egg-info/entry_points.txt
--rw-rw-r--   0 cause     (1000) cause     (1000)       47 2016-01-10 16:35:38.000000 publicsuffixlist-0.9.3/publicsuffixlist.egg-info/pbr.json
--rw-rw-r--   0 cause     (1000) cause     (1000)       36 2023-01-31 06:13:08.000000 publicsuffixlist-0.9.3/publicsuffixlist.egg-info/requires.txt
--rw-rw-r--   0 cause     (1000) cause     (1000)       17 2023-01-31 06:13:08.000000 publicsuffixlist-0.9.3/publicsuffixlist.egg-info/top_level.txt
--rw-rw-r--   0 cause     (1000) cause     (1000)      108 2023-01-31 06:13:08.513105 publicsuffixlist-0.9.3/setup.cfg
--rwxrwxr-x   0 cause     (1000) cause     (1000)     1294 2023-01-31 06:12:56.000000 publicsuffixlist-0.9.3/setup.py
+drwxrwxr-x   0 cause     (1000) cause     (1000)        0 2023-04-15 13:38:37.791960 publicsuffixlist-0.9.4/
+-rw-rw-r--   0 cause     (1000) cause     (1000)    15922 2014-11-20 12:19:18.000000 publicsuffixlist-0.9.4/LICENSE
+-rw-rw-r--   0 cause     (1000) cause     (1000)       36 2015-09-22 17:58:20.000000 publicsuffixlist-0.9.4/MANIFEST.in
+-rw-rw-r--   0 cause     (1000) cause     (1000)     4744 2023-04-15 13:38:37.791960 publicsuffixlist-0.9.4/PKG-INFO
+-rw-rw-r--   0 cause     (1000) cause     (1000)     4132 2023-04-15 13:31:58.000000 publicsuffixlist-0.9.4/README.md
+drwxrwxr-x   0 cause     (1000) cause     (1000)        0 2023-04-15 13:38:37.787960 publicsuffixlist-0.9.4/publicsuffixlist/
+-rw-rw-r--   0 cause     (1000) cause     (1000)     8433 2022-09-28 05:59:35.000000 publicsuffixlist-0.9.4/publicsuffixlist/__init__.py
+-rw-rw-r--   0 cause     (1000) cause     (1000)      917 2020-05-26 11:13:30.000000 publicsuffixlist-0.9.4/publicsuffixlist/compat.py
+-rw-rw-r--   0 cause     (1000) cause     (1000)   238005 2023-04-15 13:31:58.000000 publicsuffixlist-0.9.4/publicsuffixlist/public_suffix_list.dat
+-rw-rw-r--   0 cause     (1000) cause     (1000)    10884 2022-09-28 05:59:35.000000 publicsuffixlist-0.9.4/publicsuffixlist/test.py
+-rw-rw-r--   0 cause     (1000) cause     (1000)     4308 2021-12-16 03:54:52.000000 publicsuffixlist-0.9.4/publicsuffixlist/test_psl.txt
+-rw-rw-r--   0 cause     (1000) cause     (1000)     1662 2023-01-31 06:12:56.000000 publicsuffixlist-0.9.4/publicsuffixlist/update.py
+drwxrwxr-x   0 cause     (1000) cause     (1000)        0 2023-04-15 13:38:37.791960 publicsuffixlist-0.9.4/publicsuffixlist.egg-info/
+-rw-rw-r--   0 cause     (1000) cause     (1000)     4744 2023-04-15 13:38:37.000000 publicsuffixlist-0.9.4/publicsuffixlist.egg-info/PKG-INFO
+-rw-rw-r--   0 cause     (1000) cause     (1000)      503 2023-04-15 13:38:37.000000 publicsuffixlist-0.9.4/publicsuffixlist.egg-info/SOURCES.txt
+-rw-rw-r--   0 cause     (1000) cause     (1000)        1 2023-04-15 13:38:37.000000 publicsuffixlist-0.9.4/publicsuffixlist.egg-info/dependency_links.txt
+-rw-rw-r--   0 cause     (1000) cause     (1000)       80 2023-04-15 13:38:37.000000 publicsuffixlist-0.9.4/publicsuffixlist.egg-info/entry_points.txt
+-rw-rw-r--   0 cause     (1000) cause     (1000)       47 2016-01-10 16:35:38.000000 publicsuffixlist-0.9.4/publicsuffixlist.egg-info/pbr.json
+-rw-rw-r--   0 cause     (1000) cause     (1000)       36 2023-04-15 13:38:37.000000 publicsuffixlist-0.9.4/publicsuffixlist.egg-info/requires.txt
+-rw-rw-r--   0 cause     (1000) cause     (1000)       17 2023-04-15 13:38:37.000000 publicsuffixlist-0.9.4/publicsuffixlist.egg-info/top_level.txt
+-rw-rw-r--   0 cause     (1000) cause     (1000)      108 2023-04-15 13:38:37.791960 publicsuffixlist-0.9.4/setup.cfg
+-rwxrwxr-x   0 cause     (1000) cause     (1000)     1438 2023-04-15 13:31:58.000000 publicsuffixlist-0.9.4/setup.py
```

### Comparing `publicsuffixlist-0.9.3/LICENSE` & `publicsuffixlist-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `publicsuffixlist-0.9.3/PKG-INFO` & `publicsuffixlist-0.9.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: publicsuffixlist
-Version: 0.9.3
-Summary: publicsuffixlist implement
-Home-page: https://github.com/ko-zu/psl
-Author: ko-zu
-Author-email: causeless@gmail.com
-License: MPL-2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Topic :: Internet :: Name Service (DNS)
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Operating System :: OS Independent
-Requires-Python: >=2.6
-Description-Content-Type: text/markdown
-Provides-Extra: update
-Provides-Extra: readme
-License-File: LICENSE
-
 publicsuffixlist
 ===
 
 [Public Suffix List](https://publicsuffix.org/) parser implementation for Python 2.6+/3.x.
 
 - Compliant with [TEST DATA](https://raw.githubusercontent.com/publicsuffix/list/master/tests/test_psl.txt)
 - Support IDN (unicode or punycoded).
@@ -129,12 +110,19 @@
 ===
 
 - This module is licensed under Mozilla Public License 2.0.
 - Public Suffix List maintained by Mozilla Foundation is licensed under Mozilla Public License 2.0.
 - PSL testcase dataset is public domain (CC0).
 
 
+Development / Packaging
+===
+This module and its packaging workflow are maintained in the author's repository located at https://github.com/ko-zu/psl.
+A new package, which includes the latest PSL file, is automatically generated and uploaded to PyPI.
+The last part of the version number represents the release date, for instance, `0.10.1.20230331`.
+
+
 Source / Link
 ===
 
 - Git repository on GitHub (https://github.com/ko-zu/psl)
 - PyPI (https://pypi.org/project/publicsuffixlist/)
```

### Comparing `publicsuffixlist-0.9.3/publicsuffixlist/__init__.py` & `publicsuffixlist-0.9.4/publicsuffixlist/__init__.py`

 * *Files identical despite different names*

### Comparing `publicsuffixlist-0.9.3/publicsuffixlist/compat.py` & `publicsuffixlist-0.9.4/publicsuffixlist/compat.py`

 * *Files identical despite different names*

### Comparing `publicsuffixlist-0.9.3/publicsuffixlist/public_suffix_list.dat` & `publicsuffixlist-0.9.4/publicsuffixlist/public_suffix_list.dat`

 * *Files 6% similar despite different names*

```diff
@@ -376,19 +376,37 @@
 edu.bi
 or.bi
 org.bi
 
 // biz : https://en.wikipedia.org/wiki/.biz
 biz
 
-// bj : https://en.wikipedia.org/wiki/.bj
+// bj : https://nic.bj/bj-suffixes.txt
+// submitted by registry <contact@nic.bj>
 bj
-asso.bj
-barreau.bj
-gouv.bj
+africa.bj
+agro.bj
+architectes.bj
+assur.bj
+avocats.bj
+co.bj
+com.bj
+eco.bj
+econo.bj
+edu.bj
+info.bj
+loisirs.bj
+money.bj
+net.bj
+org.bj
+ote.bj
+resto.bj
+restaurant.bj
+tourism.bj
+univ.bj
 
 // bm : http://www.bermudanic.bm/dnr-text.txt
 bm
 com.bm
 edu.bm
 gov.bm
 net.bm
@@ -1029,24 +1047,23 @@
 net.fm
 org.fm
 fm
 
 // fo : https://en.wikipedia.org/wiki/.fo
 fo
 
-// fr : http://www.afnic.fr/
-// domaines descriptifs : https://www.afnic.fr/medias/documents/Cadre_legal/Afnic_Naming_Policy_12122016_VEN.pdf
+// fr : https://www.afnic.fr/ https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 fr
 asso.fr
 com.fr
 gouv.fr
 nom.fr
 prd.fr
 tm.fr
-// domaines sectoriels : https://www.afnic.fr/en/products-and-services/the-fr-tld/sector-based-fr-domains-4.html
+// Former "domaines sectoriels", still registration suffixes
 aeroport.fr
 avocat.fr
 avoues.fr
 cci.fr
 chambagri.fr
 chirurgiens-dentistes.fr
 experts-comptables.fr
@@ -4048,563 +4065,16 @@
 net.mu
 org.mu
 gov.mu
 ac.mu
 co.mu
 or.mu
 
-// museum : http://about.museum/naming/
-// http://index.museum/
+// museum : https://welcome.museum/wp-content/uploads/2018/05/20180525-Registration-Policy-MUSEUM-EN_VF-2.pdf https://welcome.museum/buy-your-dot-museum-2/
 museum
-academy.museum
-agriculture.museum
-air.museum
-airguard.museum
-alabama.museum
-alaska.museum
-amber.museum
-ambulance.museum
-american.museum
-americana.museum
-americanantiques.museum
-americanart.museum
-amsterdam.museum
-and.museum
-annefrank.museum
-anthro.museum
-anthropology.museum
-antiques.museum
-aquarium.museum
-arboretum.museum
-archaeological.museum
-archaeology.museum
-architecture.museum
-art.museum
-artanddesign.museum
-artcenter.museum
-artdeco.museum
-arteducation.museum
-artgallery.museum
-arts.museum
-artsandcrafts.museum
-asmatart.museum
-assassination.museum
-assisi.museum
-association.museum
-astronomy.museum
-atlanta.museum
-austin.museum
-australia.museum
-automotive.museum
-aviation.museum
-axis.museum
-badajoz.museum
-baghdad.museum
-bahn.museum
-bale.museum
-baltimore.museum
-barcelona.museum
-baseball.museum
-basel.museum
-baths.museum
-bauern.museum
-beauxarts.museum
-beeldengeluid.museum
-bellevue.museum
-bergbau.museum
-berkeley.museum
-berlin.museum
-bern.museum
-bible.museum
-bilbao.museum
-bill.museum
-birdart.museum
-birthplace.museum
-bonn.museum
-boston.museum
-botanical.museum
-botanicalgarden.museum
-botanicgarden.museum
-botany.museum
-brandywinevalley.museum
-brasil.museum
-bristol.museum
-british.museum
-britishcolumbia.museum
-broadcast.museum
-brunel.museum
-brussel.museum
-brussels.museum
-bruxelles.museum
-building.museum
-burghof.museum
-bus.museum
-bushey.museum
-cadaques.museum
-california.museum
-cambridge.museum
-can.museum
-canada.museum
-capebreton.museum
-carrier.museum
-cartoonart.museum
-casadelamoneda.museum
-castle.museum
-castres.museum
-celtic.museum
-center.museum
-chattanooga.museum
-cheltenham.museum
-chesapeakebay.museum
-chicago.museum
-children.museum
-childrens.museum
-childrensgarden.museum
-chiropractic.museum
-chocolate.museum
-christiansburg.museum
-cincinnati.museum
-cinema.museum
-circus.museum
-civilisation.museum
-civilization.museum
-civilwar.museum
-clinton.museum
-clock.museum
-coal.museum
-coastaldefence.museum
-cody.museum
-coldwar.museum
-collection.museum
-colonialwilliamsburg.museum
-coloradoplateau.museum
-columbia.museum
-columbus.museum
-communication.museum
-communications.museum
-community.museum
-computer.museum
-computerhistory.museum
-comunicações.museum
-contemporary.museum
-contemporaryart.museum
-convent.museum
-copenhagen.museum
-corporation.museum
-correios-e-telecomunicações.museum
-corvette.museum
-costume.museum
-countryestate.museum
-county.museum
-crafts.museum
-cranbrook.museum
-creation.museum
-cultural.museum
-culturalcenter.museum
-culture.museum
-cyber.museum
-cymru.museum
-dali.museum
-dallas.museum
-database.museum
-ddr.museum
-decorativearts.museum
-delaware.museum
-delmenhorst.museum
-denmark.museum
-depot.museum
-design.museum
-detroit.museum
-dinosaur.museum
-discovery.museum
-dolls.museum
-donostia.museum
-durham.museum
-eastafrica.museum
-eastcoast.museum
-education.museum
-educational.museum
-egyptian.museum
-eisenbahn.museum
-elburg.museum
-elvendrell.museum
-embroidery.museum
-encyclopedic.museum
-england.museum
-entomology.museum
-environment.museum
-environmentalconservation.museum
-epilepsy.museum
-essex.museum
-estate.museum
-ethnology.museum
-exeter.museum
-exhibition.museum
-family.museum
-farm.museum
-farmequipment.museum
-farmers.museum
-farmstead.museum
-field.museum
-figueres.museum
-filatelia.museum
-film.museum
-fineart.museum
-finearts.museum
-finland.museum
-flanders.museum
-florida.museum
-force.museum
-fortmissoula.museum
-fortworth.museum
-foundation.museum
-francaise.museum
-frankfurt.museum
-franziskaner.museum
-freemasonry.museum
-freiburg.museum
-fribourg.museum
-frog.museum
-fundacio.museum
-furniture.museum
-gallery.museum
-garden.museum
-gateway.museum
-geelvinck.museum
-gemological.museum
-geology.museum
-georgia.museum
-giessen.museum
-glas.museum
-glass.museum
-gorge.museum
-grandrapids.museum
-graz.museum
-guernsey.museum
-halloffame.museum
-hamburg.museum
-handson.museum
-harvestcelebration.museum
-hawaii.museum
-health.museum
-heimatunduhren.museum
-hellas.museum
-helsinki.museum
-hembygdsforbund.museum
-heritage.museum
-histoire.museum
-historical.museum
-historicalsociety.museum
-historichouses.museum
-historisch.museum
-historisches.museum
-history.museum
-historyofscience.museum
-horology.museum
-house.museum
-humanities.museum
-illustration.museum
-imageandsound.museum
-indian.museum
-indiana.museum
-indianapolis.museum
-indianmarket.museum
-intelligence.museum
-interactive.museum
-iraq.museum
-iron.museum
-isleofman.museum
-jamison.museum
-jefferson.museum
-jerusalem.museum
-jewelry.museum
-jewish.museum
-jewishart.museum
-jfk.museum
-journalism.museum
-judaica.museum
-judygarland.museum
-juedisches.museum
-juif.museum
-karate.museum
-karikatur.museum
-kids.museum
-koebenhavn.museum
-koeln.museum
-kunst.museum
-kunstsammlung.museum
-kunstunddesign.museum
-labor.museum
-labour.museum
-lajolla.museum
-lancashire.museum
-landes.museum
-lans.museum
-läns.museum
-larsson.museum
-lewismiller.museum
-lincoln.museum
-linz.museum
-living.museum
-livinghistory.museum
-localhistory.museum
-london.museum
-losangeles.museum
-louvre.museum
-loyalist.museum
-lucerne.museum
-luxembourg.museum
-luzern.museum
-mad.museum
-madrid.museum
-mallorca.museum
-manchester.museum
-mansion.museum
-mansions.museum
-manx.museum
-marburg.museum
-maritime.museum
-maritimo.museum
-maryland.museum
-marylhurst.museum
-media.museum
-medical.museum
-medizinhistorisches.museum
-meeres.museum
-memorial.museum
-mesaverde.museum
-michigan.museum
-midatlantic.museum
-military.museum
-mill.museum
-miners.museum
-mining.museum
-minnesota.museum
-missile.museum
-missoula.museum
-modern.museum
-moma.museum
-money.museum
-monmouth.museum
-monticello.museum
-montreal.museum
-moscow.museum
-motorcycle.museum
-muenchen.museum
-muenster.museum
-mulhouse.museum
-muncie.museum
-museet.museum
-museumcenter.museum
-museumvereniging.museum
-music.museum
-national.museum
-nationalfirearms.museum
-nationalheritage.museum
-nativeamerican.museum
-naturalhistory.museum
-naturalhistorymuseum.museum
-naturalsciences.museum
-nature.museum
-naturhistorisches.museum
-natuurwetenschappen.museum
-naumburg.museum
-naval.museum
-nebraska.museum
-neues.museum
-newhampshire.museum
-newjersey.museum
-newmexico.museum
-newport.museum
-newspaper.museum
-newyork.museum
-niepce.museum
-norfolk.museum
-north.museum
-nrw.museum
-nyc.museum
-nyny.museum
-oceanographic.museum
-oceanographique.museum
-omaha.museum
-online.museum
-ontario.museum
-openair.museum
-oregon.museum
-oregontrail.museum
-otago.museum
-oxford.museum
-pacific.museum
-paderborn.museum
-palace.museum
-paleo.museum
-palmsprings.museum
-panama.museum
-paris.museum
-pasadena.museum
-pharmacy.museum
-philadelphia.museum
-philadelphiaarea.museum
-philately.museum
-phoenix.museum
-photography.museum
-pilots.museum
-pittsburgh.museum
-planetarium.museum
-plantation.museum
-plants.museum
-plaza.museum
-portal.museum
-portland.museum
-portlligat.museum
-posts-and-telecommunications.museum
-preservation.museum
-presidio.museum
-press.museum
-project.museum
-public.museum
-pubol.museum
-quebec.museum
-railroad.museum
-railway.museum
-research.museum
-resistance.museum
-riodejaneiro.museum
-rochester.museum
-rockart.museum
-roma.museum
-russia.museum
-saintlouis.museum
-salem.museum
-salvadordali.museum
-salzburg.museum
-sandiego.museum
-sanfrancisco.museum
-santabarbara.museum
-santacruz.museum
-santafe.museum
-saskatchewan.museum
-satx.museum
-savannahga.museum
-schlesisches.museum
-schoenbrunn.museum
-schokoladen.museum
-school.museum
-schweiz.museum
-science.museum
-scienceandhistory.museum
-scienceandindustry.museum
-sciencecenter.museum
-sciencecenters.museum
-science-fiction.museum
-sciencehistory.museum
-sciences.museum
-sciencesnaturelles.museum
-scotland.museum
-seaport.museum
-settlement.museum
-settlers.museum
-shell.museum
-sherbrooke.museum
-sibenik.museum
-silk.museum
-ski.museum
-skole.museum
-society.museum
-sologne.museum
-soundandvision.museum
-southcarolina.museum
-southwest.museum
-space.museum
-spy.museum
-square.museum
-stadt.museum
-stalbans.museum
-starnberg.museum
-state.museum
-stateofdelaware.museum
-station.museum
-steam.museum
-steiermark.museum
-stjohn.museum
-stockholm.museum
-stpetersburg.museum
-stuttgart.museum
-suisse.museum
-surgeonshall.museum
-surrey.museum
-svizzera.museum
-sweden.museum
-sydney.museum
-tank.museum
-tcm.museum
-technology.museum
-telekommunikation.museum
-television.museum
-texas.museum
-textile.museum
-theater.museum
-time.museum
-timekeeping.museum
-topology.museum
-torino.museum
-touch.museum
-town.museum
-transport.museum
-tree.museum
-trolley.museum
-trust.museum
-trustee.museum
-uhren.museum
-ulm.museum
-undersea.museum
-university.museum
-usa.museum
-usantiques.museum
-usarts.museum
-uscountryestate.museum
-usculture.museum
-usdecorativearts.museum
-usgarden.museum
-ushistory.museum
-ushuaia.museum
-uslivinghistory.museum
-utah.museum
-uvic.museum
-valley.museum
-vantaa.museum
-versailles.museum
-viking.museum
-village.museum
-virginia.museum
-virtual.museum
-virtuel.museum
-vlaanderen.museum
-volkenkunde.museum
-wales.museum
-wallonie.museum
-war.museum
-washingtondc.museum
-watchandclock.museum
-watch-and-clock.museum
-western.museum
-westfalen.museum
-whaling.museum
-wildlife.museum
-williamsburg.museum
-windmill.museum
-workshop.museum
-york.museum
-yorkshire.museum
-yosemite.museum
-youth.museum
-zoological.museum
-zoology.museum
-ירושלים.museum
-иком.museum
 
 // mv : https://en.wikipedia.org/wiki/.mv
 // "mv" included because, contra Wikipedia, google.mv exists.
 mv
 aero.mv
 biz.mv
 com.mv
@@ -5839,15 +5309,15 @@
 wroclaw.pl
 zachpomor.pl
 zagan.pl
 zarow.pl
 zgora.pl
 zgorzelec.pl
 
-// pm : http://www.afnic.fr/medias/documents/AFNIC-naming-policy2012.pdf
+// pm : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 pm
 
 // pn : http://www.government.pn/PnRegistry/policies.htm
 pn
 gov.pn
 co.pn
 org.pn
@@ -5937,15 +5407,15 @@
 gov.qa
 mil.qa
 name.qa
 net.qa
 org.qa
 sch.qa
 
-// re : http://www.afnic.re/obtenir/chartes/nommage-re/annexe-descriptifs
+// re : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 re
 asso.re
 com.re
 nom.re
 
 // ro : http://www.rotld.ro/
 ro
@@ -6194,15 +5664,15 @@
 // td : https://en.wikipedia.org/wiki/.td
 td
 
 // tel: https://en.wikipedia.org/wiki/.tel
 // http://www.telnic.org/
 tel
 
-// tf : https://en.wikipedia.org/wiki/.tf
+// tf : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 tf
 
 // tg : https://en.wikipedia.org/wiki/.tg
 // http://www.nic.tg/
 tg
 
 // th : https://en.wikipedia.org/wiki/.th
@@ -6813,27 +6283,27 @@
 // http://www.vunic.vu/
 vu
 com.vu
 edu.vu
 net.vu
 org.vu
 
-// wf : http://www.afnic.fr/medias/documents/AFNIC-naming-policy2012.pdf
+// wf : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 wf
 
 // ws : https://en.wikipedia.org/wiki/.ws
 // http://samoanic.ws/index.dhtml
 ws
 com.ws
 net.ws
 org.ws
 gov.ws
 edu.ws
 
-// yt : http://www.afnic.fr/medias/documents/AFNIC-naming-policy2012.pdf
+// yt : https://www.afnic.fr/wp-media/uploads/2022/12/afnic-naming-policy-2023-01-01.pdf
 yt
 
 // IDN ccTLDs
 // When submitting patches, please maintain a sort by ISO 3166 ccTLD, then
 // U-label, and follow this format:
 // // A-Label ("<Latin renderings>", <language name>[, variant info]) : <ISO 3166 ccTLD>
 // // [sponsoring org]
@@ -7167,15 +6637,15 @@
 gov.zw
 mil.zw
 org.zw
 
 
 // newGTLDs
 
-// List of new gTLDs imported from https://www.icann.org/resources/registries/gtlds/v2/gtlds.json on 2023-01-30T09:23:24Z
+// List of new gTLDs imported from https://www.icann.org/resources/registries/gtlds/v2/gtlds.json on 2023-04-14T15:13:16Z
 // This list is auto-generated, don't edit it manually.
 // aaa : 2015-02-26 American Automobile Association, Inc.
 aaa
 
 // aarp : 2015-05-21 AARP
 aarp
 
@@ -8366,15 +7836,15 @@
 
 // glass : 2013-11-07 Binky Moon, LLC
 glass
 
 // gle : 2014-07-24 Charleston Road Registry Inc.
 gle
 
-// global : 2014-04-17 Dot Global Domain Registry Limited
+// global : 2014-04-17 Identity Digital Limited
 global
 
 // globo : 2013-12-19 Globo Comunicação e Participações S.A
 globo
 
 // gmail : 2014-05-01 Charleston Road Registry Inc.
 gmail
@@ -8876,17 +8346,14 @@
 
 // limo : 2013-10-17 Binky Moon, LLC
 limo
 
 // lincoln : 2014-11-13 Ford Motor Company
 lincoln
 
-// linde : 2014-12-04 Linde Aktiengesellschaft
-linde
-
 // link : 2013-11-14 Nova Registry Ltd
 link
 
 // lipsy : 2015-06-25 Lipsy Ltd
 lipsy
 
 // live : 2014-12-04 Dog Beach, LLC
@@ -8945,17 +8412,14 @@
 
 // luxe : 2014-01-09 Registry Services, LLC
 luxe
 
 // luxury : 2013-10-17 Luxury Partners, LLC
 luxury
 
-// macys : 2015-07-31 Macys, Inc.
-macys
-
 // madrid : 2014-05-01 Comunidad de Madrid
 madrid
 
 // maif : 2014-10-02 Mutuelle Assurance Instituteur France (MAIF)
 maif
 
 // maison : 2013-12-05 Binky Moon, LLC
@@ -9287,15 +8751,15 @@
 
 // ovh : 2014-01-16 MédiaBC
 ovh
 
 // page : 2014-12-04 Charleston Road Registry Inc.
 page
 
-// panasonic : 2015-07-30 Panasonic Corporation
+// panasonic : 2015-07-30 Panasonic Holdings Corporation
 panasonic
 
 // paris : 2014-01-30 City of Paris
 paris
 
 // pars : 2014-09-04 Asia Green IT System Bilgisayar San. ve Tic. Ltd. Sti.
 pars
@@ -9449,15 +8913,15 @@
 
 // pub : 2013-12-12 Dog Beach, LLC
 pub
 
 // pwc : 2015-10-29 PricewaterhouseCoopers LLP
 pwc
 
-// qpon : 2013-11-14 dotCOOL, Inc.
+// qpon : 2013-11-14 dotQPON LLC
 qpon
 
 // quebec : 2013-12-19 PointQuébec Inc
 quebec
 
 // quest : 2015-03-26 XYZ.COM LLC
 quest
@@ -10655,28 +10119,51 @@
 adobeaemcloud.com
 *.dev.adobeaemcloud.com
 hlx.live
 adobeaemcloud.net
 hlx.page
 hlx3.page
 
+// Adobe Developer Platform : https://developer.adobe.com
+// Submitted by Jesse MacFadyen<jessem@adobe.com>
+adobeio-static.net
+adobeioruntime.net
+
 // Agnat sp. z o.o. : https://domena.pl
 // Submitted by Przemyslaw Plewa <it-admin@domena.pl>
 beep.pl
 
 // Airkit : https://www.airkit.com/
 // Submitted by Grant Cooksey <security@airkit.com>
 airkitapps.com
 airkitapps-au.com
 airkitapps.eu
 
 // Aiven: https://aiven.io/
 // Submitted by Etienne Stalmans <security@aiven.io>
 aivencloud.com
 
+// Akamai : https://www.akamai.com/
+// Submitted by Akamai Team <publicsuffixlist@akamai.com>
+akadns.net
+akamai.net
+akamai-staging.net
+akamaiedge.net
+akamaiedge-staging.net
+akamaihd.net
+akamaihd-staging.net
+akamaiorigin.net
+akamaiorigin-staging.net
+akamaized.net
+akamaized-staging.net
+edgekey.net
+edgekey-staging.net
+edgesuite.net
+edgesuite-staging.net
+
 // alboto.ca : http://alboto.ca
 // Submitted by Anton Avramov <avramov@alboto.ca>
 barsy.ca
 
 // Alces Software Ltd : http://alces-software.com
 // Submitted by Mark J. Titorenko <mark.titorenko@alces-software.com>
 *.compute.estate
@@ -10913,14 +10400,18 @@
 // Submitted by Sam Smyth <devloop@atlassian.com>
 cdn.prod.atlassian-dev.net
 
 // Authentick UG (haftungsbeschränkt) : https://authentick.net
 // Submitted by Lukas Reschke <lukas@authentick.net>
 translated.page
 
+// Autocode : https://autocode.com
+// Submitted by Jacob Lee <jacob@autocode.com>
+autocode.dev
+
 // AVM : https://avm.de
 // Submitted by Andreas Weise <a.weise@avm.de>
 myfritz.net
 
 // AVStack Pte. Ltd. : https://avstack.io
 // Submitted by Jasper Hugo <jasper@avstack.io>
 onavstack.net
@@ -11041,14 +10532,19 @@
 // Submitted by Antonio Lain <antlai@cafjs.com>
 cafjs.com
 
 // callidomus : https://www.callidomus.com/
 // Submitted by Marcus Popp <admin@callidomus.com>
 mycd.eu
 
+// Canva Pty Ltd : https://canva.com/
+// Submitted by Joel Aquilina <publicsuffixlist@canva.com>
+canva-apps.cn
+canva-apps.com
+
 // Carrd : https://carrd.co
 // Submitted by AJ <aj@carrd.co>
 drr.ac
 uwu.ai
 carrd.co
 crd.co
 ju.mp
@@ -11958,14 +11454,15 @@
 // Submitted by Aman Gupta <aman@getchannels.com>
 channelsdvr.net
 u.channelsdvr.net
 
 // Fastly Inc. : http://www.fastly.com/
 // Submitted by Fastly Security <security@fastly.com>
 edgecompute.app
+fastly-edge.com
 fastly-terrarium.com
 fastlylb.net
 map.fastlylb.net
 freetls.fastly.net
 map.fastly.net
 a.prod.fastly.net
 global.prod.fastly.net
@@ -12472,14 +11969,18 @@
 firm.ng
 gen.ng
 ltd.ng
 ngo.ng
 edu.scot
 sch.so
 
+// HostFly : https://www.ie.ua
+// Submitted by Bohdan Dub <support@hostfly.com.ua>
+ie.ua
+
 // HostyHosting (hostyhosting.com)
 hostyhosting.io
 
 // Häkkinen.fi
 // Submitted by Eero Häkkinen <Eero+psl@Häkkinen.fi>
 häkkinen.fi
 
@@ -12930,14 +12431,15 @@
 *.azurecontainer.io
 azurewebsites.net
 azure-mobile.net
 cloudapp.net
 azurestaticapps.net
 1.azurestaticapps.net
 2.azurestaticapps.net
+3.azurestaticapps.net
 centralus.azurestaticapps.net
 eastasia.azurestaticapps.net
 eastus2.azurestaticapps.net
 westeurope.azurestaticapps.net
 westus2.azurestaticapps.net
 
 // minion.systems : http://minion.systems
@@ -12996,15 +12498,27 @@
 
 // Neustar Inc.
 // Submitted by Trung Tran <Trung.Tran@neustar.biz>
 4u.com
 
 // ngrok : https://ngrok.com/
 // Submitted by Alan Shreve <alan@ngrok.com>
+ngrok.app
+ngrok-free.app
+ngrok.dev
+ngrok-free.dev
 ngrok.io
+ap.ngrok.io
+au.ngrok.io
+eu.ngrok.io
+in.ngrok.io
+jp.ngrok.io
+sa.ngrok.io
+us.ngrok.io
+ngrok.pizza
 
 // Nimbus Hosting Ltd. : https://www.nimbushosting.co.uk/
 // Submitted by Nicholas Ford <nick@nimbushosting.co.uk>
 nh-serv.co.uk
 
 // NFSN, Inc. : https://www.NearlyFreeSpeech.NET/
 // Submitted by Jeff Wheelhouse <support@nearlyfreespeech.net>
@@ -13393,14 +12907,18 @@
 // Submitted by Jeffrey Phillips Freeman <jeffrey.freeman@qoto.org>
 qoto.io
 
 // Qualifio : https://qualifio.com/
 // Submitted by Xavier De Cock <xdecock@gmail.com>
 qualifioapp.com
 
+// Quality Unit: https://qualityunit.com
+// Submitted by Vasyl Tsalko <vtsalko@qualityunit.com>
+ladesk.com
+
 // QuickBackend: https://www.quickbackend.com
 // Submitted by Dani Biro <dani@pymet.com>
 qbuser.com
 
 // Rad Web Hosting: https://radwebhosting.com
 // Submitted by Scott Claeys <s.claeys@radwebhosting.com>
 cloudsite.builders
@@ -13516,14 +13034,64 @@
 мск.рус
 орг.рус
 самара.рус
 сочи.рус
 спб.рус
 я.рус
 
+// SAKURA Internet Inc. : https://www.sakura.ad.jp/
+// Submitted by Internet Service Department <rs-vendor-ml@sakura.ad.jp>
+180r.com
+dojin.com
+sakuratan.com
+sakuraweb.com
+x0.com
+2-d.jp
+bona.jp
+crap.jp
+daynight.jp
+eek.jp
+flop.jp
+halfmoon.jp
+jeez.jp
+matrix.jp
+mimoza.jp
+ivory.ne.jp
+mail-box.ne.jp
+mints.ne.jp
+mokuren.ne.jp
+opal.ne.jp
+sakura.ne.jp
+sumomo.ne.jp
+topaz.ne.jp
+netgamers.jp
+nyanta.jp
+o0o0.jp
+rdy.jp
+rgr.jp
+rulez.jp
+s3.isk01.sakurastorage.jp
+s3.isk02.sakurastorage.jp
+saloon.jp
+sblo.jp
+skr.jp
+tank.jp
+uh-oh.jp
+undo.jp
+rs.webaccel.jp
+user.webaccel.jp
+websozai.jp
+xii.jp
+squares.net
+jpn.org
+kirara.st
+x0.to
+from.tv
+sakura.tv
+
 // Salesforce.com, Inc. https://salesforce.com/
 // Submitted by Michael Biven <mbiven@salesforce.com>
 *.builder.code.com
 *.dev-builder.code.com
 *.stg-builder.code.com
 
 // Sandstorm Development Group, Inc. : https://sandcats.io/
@@ -13668,14 +13236,17 @@
 
 // Smoove.io : https://www.smoove.io/
 // Submitted by Dan Kozak <dan@smoove.io>
 vp4.me
 
 // Snowflake Inc : https://www.snowflake.com/
 // Submitted by Faith Olapade <faith.olapade@snowflake.com>
+snowflake.app
+privatelink.snowflake.app
+streamlit.app
 streamlitapp.com
 
 // Snowplow Analytics : https://snowplowanalytics.com/
 // Submitted by Ian Streeter <ian@snowplowanalytics.com>
 try-snowplow.com
 
 // SourceHut : https://sourcehut.org
@@ -13943,14 +13514,18 @@
 // UDR Limited : http://www.udr.hk.com
 // Submitted by registry <hostmaster@udr.hk.com>
 hk.com
 hk.org
 ltd.hk
 inc.hk
 
+// UK Intis Telecom LTD : https://it.com
+// Submitted by ITComdomains <to@it.com>
+it.com
+
 // UNIVERSAL DOMAIN REGISTRY : https://www.udr.org.yt/
 // see also: whois -h whois.udr.org.yt help
 // Submitted by Atanunu Igbunuroghene <publicsuffixlist@udr.org.yt>
 name.pm
 sch.tf
 biz.wf
 sch.wf
```

### Comparing `publicsuffixlist-0.9.3/publicsuffixlist/test.py` & `publicsuffixlist-0.9.4/publicsuffixlist/test.py`

 * *Files identical despite different names*

### Comparing `publicsuffixlist-0.9.3/publicsuffixlist/test_psl.txt` & `publicsuffixlist-0.9.4/publicsuffixlist/test_psl.txt`

 * *Files identical despite different names*

### Comparing `publicsuffixlist-0.9.3/publicsuffixlist/update.py` & `publicsuffixlist-0.9.4/publicsuffixlist/update.py`

 * *Files identical despite different names*

### Comparing `publicsuffixlist-0.9.3/publicsuffixlist.egg-info/PKG-INFO` & `publicsuffixlist-0.9.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publicsuffixlist
-Version: 0.9.3
+Version: 0.9.4
 Summary: publicsuffixlist implement
 Home-page: https://github.com/ko-zu/psl
 Author: ko-zu
 Author-email: causeless@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -129,12 +129,19 @@
 ===
 
 - This module is licensed under Mozilla Public License 2.0.
 - Public Suffix List maintained by Mozilla Foundation is licensed under Mozilla Public License 2.0.
 - PSL testcase dataset is public domain (CC0).
 
 
+Development / Packaging
+===
+This module and its packaging workflow are maintained in the author's repository located at https://github.com/ko-zu/psl.
+A new package, which includes the latest PSL file, is automatically generated and uploaded to PyPI.
+The last part of the version number represents the release date, for instance, `0.10.1.20230331`.
+
+
 Source / Link
 ===
 
 - Git repository on GitHub (https://github.com/ko-zu/psl)
 - PyPI (https://pypi.org/project/publicsuffixlist/)
```

