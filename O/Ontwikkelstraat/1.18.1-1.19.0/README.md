# Comparing `tmp/ontwikkelstraat-1.18.1.tar.gz` & `tmp/ontwikkelstraat-1.19.0.tar.gz`

## Comparing `ontwikkelstraat-1.18.1.tar` & `ontwikkelstraat-1.19.0.tar`

### file list

```diff
@@ -1,971 +1,971 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/.dockerignore
--rw-r--r--   0        0        0    52207 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/CHANGELOG.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/__init__.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/bundle-lts.yaml
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/bundle.yaml
--rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docker-compose.yml
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/mkdocs.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/requirements.in
--rw-r--r--   0        0        0    25604 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/tasks.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/architectuur-vanuit-netwerk-perspectief.md
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-installeer-je-omgevingen.md
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-testen-we-de-frontend.md
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-werken-verchillende-applicatie-versies.md
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-werken-we-met-branches.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-werken-we-met-ssh.md
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-werkt-de-backup-en-restore.md
--rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-werkt-de-frontend.md
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-werkt-locust.md
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/hoe-wordt-een-server-geprovisioned.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/index.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/mkdocs.md
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/over-deze-documentatie.md
--rw-r--r--   0        0        0    78735 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/playwright_img.png
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/sequence.puml
--rw-r--r--   0        0        0   314339 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/versiebeheer-miro-bord.png
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-applog.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-celery.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-cmsx.md
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-de-bundler.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-de-feature-omgeving.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-de-fica-omgeving.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-de-workbench.md
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-docker-compose.md
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-docker.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-dotenv.md
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-een-omgeving.md
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-fabric.md
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-fragmentx.md
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-ghost.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-git.md
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-invoke.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-locust.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-lts.md
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-migrate.md
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-multipass.md
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-pip-compile.md
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-playwright.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-postgres.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-py4web.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-redis.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-restic.md
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-treafik.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-web2py.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-is-xonsh.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/docs/wat-zijn-de-core-libraries.md
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/requirements.in
--rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/requirements.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/.env.sample
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Ghost blog searcher.ipynb
--rw-r--r--   0        0        0    30289 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Kladblaadje statistieken.ipynb
--rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Knutselwerk tags en items.ipynb
--rw-r--r--   0        0        0   962690 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/LOF-ghost-archief.ipynb
--rw-r--r--   0        0        0   103193 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Leids aanbod statistieken.ipynb
--rw-r--r--   0        0        0    13322 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Nieuwe sticker toevoegen.ipynb
--rw-r--r--   0        0        0    19551 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Regulier Tag Ondehoud.ipynb
--rw-r--r--   0        0        0     9286 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Romy's database hoofd ontplof pagina.ipynb
--rw-r--r--   0        0        0    44883 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Snippets en voorbeelden.ipynb
--rw-r--r--   0        0        0   154863 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Tags and database tuning.ipynb
--rw-r--r--   0        0        0    21225 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Widgets.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/__init__.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/__init__edwh__new.ipynb
--rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/__init__edwh__notebooks.ipynb
--rw-r--r--   0        0        0    41002 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/ghost.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/handig.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/item_search_quicky.ipynb
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/nocodb.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/organisations_naar_changelog.ipynb
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/poging_plpython3.ipynb
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/quicky_tags_editen.ipynb
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/sqlite_to_pydal.ipynb
--rw-r--r--   0        0        0   140777 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/ticket 248.ipynb
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/DUO data importer - via API.ipynb
--rw-r--r--   0        0        0    32676 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/DUO data importer - via datadump.ipynb
--rw-r--r--   0        0        0    15029 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/Staging DUO data to effdted organisations.ipynb
--rw-r--r--   0        0        0    68495 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/Untitled.ipynb
--rw-r--r--   0        0        0    62640 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/scholenopdekaart data importer.ipynb
--rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/views.sql
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/db/readme.md
--rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/20230213 vo onderwijstype.ipynb
--rw-r--r--   0        0        0    10759 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/21.11.25-Omgeving Leiden verhuizen.ipynb
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/IOL_import.ipynb
--rw-r--r--   0        0        0   312854 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/Leids aanbod uit Ghost overzetten.ipynb
--rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/Locatiegegevens aan Organisatie.ipynb
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/eddie-icon.png
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/opruimen_van_eddie_tags.ipynb
--rw-r--r--   0        0        0    86596 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/qrcode demo.ipynb
--rw-r--r--   0        0        0    45040 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/caching/caching-icm-shared-code.ipynb
--rw-r--r--   0        0        0    40547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/caching/caching.ipynb
--rw-r--r--   0        0        0    28437 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/sync/federation.ipynb
--rw-r--r--   0        0        0    31541 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/jupyterlab/notebooks/sync/synchronize.ipynb
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/locust/docker-compose.yml
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/locust/locust_static_ghost.py
--rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/locust/locustfile.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/migrate/Dockerfile
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/migrate/requirements.in
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/migrate/requirements.txt
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/migrate/data/README.md
--rw-r--r--   0        0        0    67927 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/migrate/data/empty.sql
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/migrate/flags/README.txt
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/playwright_test/conftest.py
--rw-r--r--   0        0        0    52511 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/playwright_test/test_static_ghost.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/playwright_test/screenshots/delete_all_screenshots.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/Dockerfile
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/py4web_bjoern.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/py4web_wsgi.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/requirements.in
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/requirements.txt
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/c/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/c/static/README.md
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/__init__.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/demo.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/fixtures.py
--rw-r--r--   0        0        0    13812 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/handlebars.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/opengraph.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/settings.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/src/sass/main.scss
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/README.md
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/fonts.css
--rw-r--r--   0        0        0  1497327 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/mystyles.css
--rw-r--r--   0        0        0    62128 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/banner.webp
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/boy.png
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-by.svg
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-general.svg
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-nc-eu.svg
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-nd.svg
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-remix.svg
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-sa.svg
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-share.svg
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-zero.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/chevron-up.svg
--rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/de-pionier.png
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/elders.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/email.svg
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/grootte.svg
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/hier.svg
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/hs-leiden.png
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/icon.png
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/info.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/kennis.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/locatie.svg
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/logo.png
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/onderwijsniveau.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/onderwijstype.svg
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/pd.svg
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/pencil-solid.svg
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/profiel.svg
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/seal.png
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/user-solid.svg
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/users-solid.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/wetenschappelijk.svg
--rw-r--r--   0        0        0   278644 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/_hyperscript_w9y-0.9.3.min.js
--rw-r--r--   0        0        0   300008 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/_hyperscript_w9y-0.9.5-dev.min.js
--rw-r--r--   0        0        0   290107 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/_hyperscript_w9y-dev.min.js
--rw-r--r--   0        0        0   295499 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/_hyperscript_w9y.js
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/behaviors._hs
--rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/browser-report.js
--rw-r--r--   0        0        0    19796 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/bulma.js
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/commands._hs
--rw-r--r--   0        0        0   129599 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/htmx.js
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/htmx_extend.js
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/javascript_dependencies.js
--rw-r--r--   0        0        0    33273 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/leaflet-providers.js
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/activiteiten.hbs
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/attribution.hbs
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/component.hbs
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/demo.hbs
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/demo_component.hbs
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/demo_template.hbs
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/extern.hbs
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/hotspots.hbs
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/index.hbs
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/item.hbs
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/item.html
--rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/leiden.hbs
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/loading-error.html
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/ratings.hbs
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/school.hbs
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/school.html
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/school_praktijkoverzicht.hbs
--rw-r--r--   0        0        0    21455 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/template-item.html
--rw-r--r--   0        0        0    26740 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/template.hbs
--rw-r--r--   0        0        0    26702 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/template.html
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/template_minimal.hbs
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/user.hbs
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/user.html
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/__init__.py
--rw-r--r--   0        0        0    23159 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/backend_support.py
--rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/common.py
--rw-r--r--   0        0        0    53219 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/controllers.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/fixtures.py
--rw-r--r--   0        0        0    12261 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/handlebars.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/helpers.py
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/hotspots.py
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/models.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/requirements.txt
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/settings.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/tasks.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/databases/README.md
--rw-r--r--   0        0        0  1050756 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/databases/plaatsen.json
--rw-r--r--   0        0        0   812804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/databases/slugified_plaatsen.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/README.md
--rw-r--r--   0        0        0  1750102 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/css/bundled-latest.css
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/css/no.css
--rw-r--r--   0        0        0    62128 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/banner.webp
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/boy.png
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-by.svg
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-general.svg
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-nc-eu.svg
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-nd.svg
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-remix.svg
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-sa.svg
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-share.svg
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-zero.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/chevron-up.svg
--rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/de-pionier.png
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/elders.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/email.svg
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/grootte.svg
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/hier.svg
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/hs-leiden.png
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/icon.png
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/info.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/kennis.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/locatie.svg
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/onderwijsniveau.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/onderwijstype.svg
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/pd.svg
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/pencil-solid.svg
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/profiel.svg
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/seal.png
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/user-solid.svg
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/users-solid.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/wetenschappelijk.svg
--rw-r--r--   0        0        0    50592 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/a.png
--rw-r--r--   0        0        0    32479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/b.png
--rw-r--r--   0        0        0    52288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/c.png
--rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/d.png
--rw-r--r--   0        0        0    35976 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/e.png
--rw-r--r--   0        0        0    15775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/f.png
--rw-r--r--   0        0        0    42655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/g.png
--rw-r--r--   0        0        0    26280 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/h.png
--rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/i.png
--rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/j.png
--rw-r--r--   0        0        0    35274 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/k.png
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/l.png
--rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/m.png
--rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/n.png
--rw-r--r--   0        0        0    27075 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/o.png
--rw-r--r--   0        0        0    33183 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/p.png
--rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/q.png
--rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/r.png
--rw-r--r--   0        0        0    46853 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/s.png
--rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/t.png
--rw-r--r--   0        0        0    21505 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/u.png
--rw-r--r--   0        0        0    42804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/v.png
--rw-r--r--   0        0        0    45793 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/w.png
--rw-r--r--   0        0        0    29958 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/x.png
--rw-r--r--   0        0        0    35670 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/y.png
--rw-r--r--   0        0        0    23193 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/z.png
--rw-r--r--   0        0        0   156808 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/js/bundled-latest.js
--rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/js/utils.js
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/README.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/active-filters.hbs
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/active_filters.html
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth.html
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/component_loader.html
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/demo.hbs
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/external_tiles.hbs
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/external_tiles.html
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/filter-with-active.hbs
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/filter-with-active.html
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/filter.hbs
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/filter.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/generic.html
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/hotspots.hbs
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/hotspots.html
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/index.html
--rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/item.hbs
--rw-r--r--   0        0        0    42192 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/item.html
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/layout.html
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/list_items.hbs
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/menu.hbs
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/menu.html
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/modals.hbs
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/modals.html
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/notification.hbs
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/notification.html
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/page_header.hbs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/quick_filter.hbs
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/quick_filter.html
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/rating_form.hbs
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/rating_results.hbs
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/school.hbs
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/school.html
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/school_praktijkoverzicht.hbs
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/school_praktijkoverzicht.html
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/simple_analytics.html
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/tiles.hbs
--rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/tiles.html
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/user.hbs
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/user.html
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/email_validate.hbs
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/email_validate.html
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/login.hbs
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/login.html
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/no_cookies.html
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/recover.hbs
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/recover.html
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/register1.hbs
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/register1.html
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/register2.hbs
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/register2.html
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/component/datalist_plaatsen.hbs
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/component/datalist_plaatsen.html
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/component/datalist_scholen.hbs
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/component/datalist_scholen.html
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filterbuttons.hbs
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filterbuttons.html
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filtermenu-modal.hbs
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filtermenu-modal.html
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filtermenu.hbs
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filtermenu.html
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/translations/empty.dir
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/translations/it.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/fragmentx/uploads/empty.dir
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/__init__.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/common.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/controllers.py
--rw-r--r--   0        0        0    12694 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/handlebars.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/helpers.py
--rw-r--r--   0        0        0    32577 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/klassen_enquete.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/settings.py
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/static/css/no.css
--rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/static/js/utils.js
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/klassen_index.html
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/layout.html
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/enquete_uitslag.hbs
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/stapel.hbs
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/thema_uitleg.hbs
--rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/thema_uitleg_schoolleider.hbs
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/verdieping.hbs
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/vraag.hbs
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/__init__.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/demo.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/fixtures.py
--rw-r--r--   0        0        0    13812 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/handlebars.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/opengraph.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/settings.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/src/sass/main.scss
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/README.md
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/fonts.css
--rw-r--r--   0        0        0  1497263 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/mystyles.css
--rw-r--r--   0        0        0    62128 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/banner.webp
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/boy.png
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/cc-by.svg
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/cc-general.svg
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/cc-sa.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/chevron-up.svg
--rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/de-pionier.png
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/elders.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/email.svg
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/grootte.svg
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/hier.svg
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/hs-leiden.png
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/info.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/kennis.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/locatie.svg
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/logo.png
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/onderwijsniveau.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/onderwijstype.svg
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/profiel.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/wetenschappelijk.svg
--rw-r--r--   0        0        0   278644 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-0.9.3.min.js
--rw-r--r--   0        0        0   300008 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-0.9.5-dev.min.js
--rw-r--r--   0        0        0   290107 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-dev.min.js
--rw-r--r--   0        0        0   295499 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/_hyperscript_w9y.js
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/behaviors._hs
--rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/browser-report.js
--rw-r--r--   0        0        0    19796 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/bulma.js
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/commands._hs
--rw-r--r--   0        0        0   129599 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/htmx.js
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/htmx_extend.js
--rw-r--r--   0        0        0    16194 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/javascript_dependencies.js
--rw-r--r--   0        0        0    33273 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/leaflet-providers.js
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/activiteiten.hbs
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/attribution.hbs
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/component.hbs
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/demo.hbs
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/demo_component.hbs
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/demo_template.hbs
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/extern.hbs
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/hotspots.hbs
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/index.hbs
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/item.hbs
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/item.html
--rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/leiden.hbs
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/loading-error.html
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/ratings.hbs
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/school.hbs
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/school.html
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/school_praktijkoverzicht.hbs
--rw-r--r--   0        0        0    67801 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/template-item.html
--rw-r--r--   0        0        0    90095 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/template.hbs
--rw-r--r--   0        0        0    91770 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/template.html
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/template_minimal.hbs
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/user.hbs
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/user.html
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/jwt_demo/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/__init__.py
--rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/common.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/controllers.py
--rw-r--r--   0        0        0    41077 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/ghost.py
--rw-r--r--   0        0        0    14685 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/handlebars.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/models.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/settings.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/tasks.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/databases/README.md
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/static/README.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/templates/index.hbs
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/__init__.py
--rw-r--r--   0        0        0    23159 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/backend_support.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/common.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/common_lts.py
--rw-r--r--   0        0        0    51846 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/controllers.py
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/fixtures.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/fixtures_lts.py
--rw-r--r--   0        0        0    19044 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/graphql_support.py
--rw-r--r--   0        0        0    15020 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/handlebars.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/helpers.py
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/hotspots.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/klassen_controllers.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/klassen_enquete.py
--rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/lts_controllers.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/markdown_template.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/models.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/models_lts.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/requirements.txt
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/settings.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/tasks.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/databases/README.md
--rw-r--r--   0        0        0  5011320 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/databases/lts_assets.sql
--rw-r--r--   0        0        0  1050756 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/databases/plaatsen.json
--rw-r--r--   0        0        0   812804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/databases/slugified_plaatsen.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/README.md
--rw-r--r--   0        0        0  1750102 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/css/bundled-1.0.0.css
--rw-r--r--   0        0        0  1748035 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/css/bundled.css
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/css/no.css
--rw-r--r--   0        0        0    62128 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/banner.webp
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/boy.png
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-by.svg
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-general.svg
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-nc-eu.svg
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-nd.svg
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-remix.svg
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-sa.svg
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-share.svg
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-zero.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/chevron-up.svg
--rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/de-pionier.png
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/elders.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/email.svg
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/grootte.svg
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/hier.svg
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/hs-leiden.png
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/icon.png
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/info.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/kennis.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/locatie.svg
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/onderwijsniveau.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/onderwijstype.svg
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/pd.svg
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/pencil-solid.svg
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/profiel.svg
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/seal.png
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/user-solid.svg
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/users-solid.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/wetenschappelijk.svg
--rw-r--r--   0        0        0    50592 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/a.png
--rw-r--r--   0        0        0    32479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/b.png
--rw-r--r--   0        0        0    52288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/c.png
--rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/d.png
--rw-r--r--   0        0        0    35976 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/e.png
--rw-r--r--   0        0        0    15775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/f.png
--rw-r--r--   0        0        0    42655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/g.png
--rw-r--r--   0        0        0    26280 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/h.png
--rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/i.png
--rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/j.png
--rw-r--r--   0        0        0    35274 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/k.png
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/l.png
--rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/m.png
--rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/n.png
--rw-r--r--   0        0        0    27075 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/o.png
--rw-r--r--   0        0        0    33183 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/p.png
--rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/q.png
--rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/r.png
--rw-r--r--   0        0        0    46853 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/s.png
--rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/t.png
--rw-r--r--   0        0        0    21505 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/u.png
--rw-r--r--   0        0        0    42804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/v.png
--rw-r--r--   0        0        0    45793 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/w.png
--rw-r--r--   0        0        0    29958 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/x.png
--rw-r--r--   0        0        0    35670 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/y.png
--rw-r--r--   0        0        0    23193 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/z.png
--rw-r--r--   0        0        0   156294 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/js/bundled-1.0.0.js
--rw-r--r--   0        0        0   156483 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/js/bundled.js
--rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/static/js/utils.js
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/README.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/active-filters.hbs
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/active_filters.html
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth.html
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/changelog.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component_loader.html
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/demo.hbs
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/documentatie.md
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/email_registration_form.hbs
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/email_registration_form.html
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/enquete_uitslag.hbs
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/external_tiles.hbs
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/external_tiles.html
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/filter-with-active.hbs
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/filter-with-active.html
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/filter.hbs
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/filter.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/generic.html
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/hotspots.hbs
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/hotspots.html
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/index.html
--rw-r--r--   0        0        0    28247 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/item.hbs
--rw-r--r--   0        0        0    32978 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/item.html
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/klassen_index.html
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/layout.html
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/list_items.hbs
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/menu.hbs
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/menu.html
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/modals.hbs
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/modals.html
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/notification.hbs
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/notification.html
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/page_header.hbs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/quick_filter.hbs
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/quick_filter.html
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/rating_form.hbs
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/rating_results.hbs
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/school.hbs
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/school.html
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/school_praktijkoverzicht.hbs
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/school_praktijkoverzicht.html
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/stapel.hbs
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/thema_uitleg.hbs
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/tiles.hbs
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/tiles.html
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/user.hbs
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/user.html
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/vraag.hbs
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/email_validate.hbs
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/email_validate.html
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/login.hbs
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/login.html
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/recover.hbs
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/recover.html
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/register1.hbs
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/register1.html
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/register2.hbs
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/register2.html
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/danger.hbs
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/danger.html
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/datalist_plaatsen.hbs
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/datalist_plaatsen.html
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/datalist_scholen.hbs
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/datalist_scholen.html
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/success.hbs
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/success.html
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/warning.hbs
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/component/warning.html
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/layouts/generic.hbs
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/layouts/markdown.html
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_1.html
--rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_2.html
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_3.html
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_layout.html
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_tags.html
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/demo.html
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/demo_template.html
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/manage.html
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/manage_grid.html
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/manage_groups.html
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filterbuttons.hbs
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filterbuttons.html
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filtermenu-modal.hbs
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filtermenu-modal.html
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filtermenu.hbs
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filtermenu.html
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/translations/empty.dir
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/translations/it.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/lts/uploads/empty.dir
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/__init__.py
--rw-r--r--   0        0        0    23159 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/backend_support.py
--rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/common.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/controllers.py
--rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/fixtures.py
--rw-r--r--   0        0        0    12261 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/handlebars.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/helpers.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/requirements.txt
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/settings.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/tasks.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/databases/README.md
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/README.md
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/LEF logo.svg
--rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/Onderwijsindeleidseregio logo.svg
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/icon.png
--rw-r--r--   0        0        0    50592 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/a.png
--rw-r--r--   0        0        0    32479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/b.png
--rw-r--r--   0        0        0    52288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/c.png
--rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/d.png
--rw-r--r--   0        0        0    35976 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/e.png
--rw-r--r--   0        0        0    15775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/f.png
--rw-r--r--   0        0        0    42655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/g.png
--rw-r--r--   0        0        0    26280 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/h.png
--rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/i.png
--rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/j.png
--rw-r--r--   0        0        0    35274 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/k.png
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/l.png
--rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/m.png
--rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/n.png
--rw-r--r--   0        0        0    27075 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/o.png
--rw-r--r--   0        0        0    33183 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/p.png
--rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/q.png
--rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/r.png
--rw-r--r--   0        0        0    46853 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/s.png
--rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/t.png
--rw-r--r--   0        0        0    21505 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/u.png
--rw-r--r--   0        0        0    42804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/v.png
--rw-r--r--   0        0        0    45793 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/w.png
--rw-r--r--   0        0        0    29958 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/x.png
--rw-r--r--   0        0        0    35670 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/y.png
--rw-r--r--   0        0        0    23193 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/z.png
--rw-r--r--   0        0        0     8763 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/templates/narrowcasting.html
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/translations/empty.dir
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/translations/it.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/uploads/empty.dir
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/restart/__init__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/restart/static/README.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/restart/static/favicon.ico
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/__init__.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/common.py
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/controllers.py
--rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/handlebars.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/models.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/settings.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/tasks.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/databases/README.md
--rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/databases/dna.csv
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/static/README.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/card.hbs
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/ghost.hbs
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/index.hbs
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/uitslag.hbs
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/vraag.hbs
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/py4web/uploaded_attachments/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/__init__.py
--rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/data_model.py
--rw-r--r--   0        0        0    69719 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/migrations.py
--rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/tags.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/asink.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/celerysink.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/diskcachesink.py
--rw-r--r--   0        0        0    14089 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/signalemitter.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/sink.py
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/tasks.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/__init__.py
--rw-r--r--   0        0        0    94817 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/engine.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/ntfy_sh.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/opengraph.py
--rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/support.py
--rw-r--r--   0        0        0    21771 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/tasks.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/jwt_tools/__init__.py
--rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/jwt_tools/jwt_py4web.py
--rw-r--r--   0        0        0     6934 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/jwt_tools/jwt_web2py.py
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/jwt_tools/shared.py
--rw-r--r--   0        0        0    18276 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/pgcache/__init__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/pgcache/clean.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/pgcache/define_models.py
--rw-r--r--   0        0        0     8712 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/sync/__init__.py
--rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/shared_code/edwh/core/web2py_tools/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/Dockerfile
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/requirements.in
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/requirements.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/routes.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/readme.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/ABOUT
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/LICENSE
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/progress.log
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/routes.example.py
--rw-r--r--   0        0        0    27197 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/controllers/appadmin.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/controllers/default.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/cron/crontab
--rw-r--r--   0        0        0    16269 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/ar.py
--rw-r--r--   0        0        0    15922 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/ca.py
--rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/cs.py
--rw-r--r--   0        0        0    16378 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/de.py
--rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/en.py
--rw-r--r--   0        0        0    16113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/es.py
--rw-r--r--   0        0        0    15937 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/fr-ca.py
--rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/fr.py
--rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/hi.py
--rw-r--r--   0        0        0    15342 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/hu.py
--rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/id.py
--rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/it.py
--rw-r--r--   0        0        0    19085 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/my-mm.py
--rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/my.py
--rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/nl.py
--rw-r--r--   0        0        0    15452 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/pl.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/plural-cs.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/plural-en.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/plural-es.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/plural-ru.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/plural-uk.py
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/pt-br.py
--rw-r--r--   0        0        0    15449 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/pt.py
--rw-r--r--   0        0        0    15584 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/ro.py
--rw-r--r--   0        0        0    16418 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/ru.py
--rw-r--r--   0        0        0    15548 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/sk.py
--rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/tr.py
--rw-r--r--   0        0        0    18665 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/uk.py
--rw-r--r--   0        0        0    15285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/zh-cn.py
--rw-r--r--   0        0        0    15437 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/zh-tw.py
--rw-r--r--   0        0        0    15437 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/zh.py
--rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/models/db.py
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/models/menu.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/modules/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/private/appconfig.ini
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/403.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/404.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/500.html
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/503.html
--rw-r--r--   0        0        0   144877 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   551641 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/bootstrap.min.css.map
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/calendar.css
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/web2py-bootstrap4.css
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/web2py.css
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/images/facebook.png
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/images/favicon.ico
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/images/favicon.png
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/images/gplus-32.png
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/images/twitter.png
--rw-r--r--   0        0        0   238247 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/analytics.min.js
--rw-r--r--   0        0        0    67742 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   273872 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0    51765 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/calendar.js
--rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/jquery.js
--rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/modernizr-2.8.3.min.js
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/web2py-bootstrap4.js
--rw-r--r--   0        0        0    37138 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/web2py.js
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/__init__.py
--rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/appadmin.html
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.csv
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.html
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.ics
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.jsonp
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.load
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.map
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.pdf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.rss
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.xml
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/layout.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/web2py_ajax.html
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/default/index.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/default/netwerken.html
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/default/socialmedia.html
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/default/user.html
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/.gitignore
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/ABOUT
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/LICENSE
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/__init__.py
--rw-r--r--   0        0        0   743011 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/errors.tgz
--rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/progress.log
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/requirements.txt
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/routes.example.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/api.py
--rw-r--r--   0        0        0    26987 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/appadmin.py
--rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/applog.py
--rw-r--r--   0        0        0    63711 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/default.py
--rw-r--r--   0        0        0    27300 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/dv_appadmin.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/jwt_auth.py
--rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/organisations.py
--rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/plugin_comments.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/scratch.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/webtest_support.py
--rw-r--r--   0        0        0    33606 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/workbench.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/cron/crontab
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/cron/crontab.example
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_apply_to_all_items.table
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_contact.table
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_dod_rule.table
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item.table
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_dod_rule.table
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_question.table
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_tag.table
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_plugin_comments_comment.table
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_question.table
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_source_file.table
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_tag_dod_rule.table
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_tag_question.table
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_cas.table
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_event.table
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_group.table
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_permission.table
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_run.table
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_task.table
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_task_deps.table
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_worker.table
--rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/sql.log
--rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/storage.sqlite
--rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/workbench.sqlite
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/functional_test/readme.md
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/functional_test/requirements.txt
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/functional_test/test.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/functional_test/tools.py
--rw-r--r--   0        0        0    27990 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/ca.py
--rw-r--r--   0        0        0    27762 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/cs.py
--rw-r--r--   0        0        0    11394 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/de.py
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/en.py
--rw-r--r--   0        0        0    25538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/es.py
--rw-r--r--   0        0        0    12596 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/fr-ca.py
--rw-r--r--   0        0        0    12483 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/fr.py
--rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/hi.py
--rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/hu.py
--rw-r--r--   0        0        0    17432 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/id.py
--rw-r--r--   0        0        0    13544 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/it.py
--rw-r--r--   0        0        0    19957 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/my-mm.py
--rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/my.py
--rw-r--r--   0        0        0    29472 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/nl.py
--rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/pl.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/plural-cs.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/plural-en.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/plural-es.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/plural-ru.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/plural-uk.py
--rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/pt-br.py
--rw-r--r--   0        0        0    10738 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/pt.py
--rw-r--r--   0        0        0    21571 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/ro.py
--rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/ru.py
--rw-r--r--   0        0        0    10469 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/sk.py
--rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/tr.py
--rw-r--r--   0        0        0    17857 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/uk.py
--rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/zh-cn.py
--rw-r--r--   0        0        0    14367 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/zh-tw.py
--rw-r--r--   0        0        0    13777 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/zh.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/aaa_400_better_error_messages.py
--rw-r--r--   0        0        0    16353 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/aaa_500_checkbox_widget.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/article_importers.py
--rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/db.py
--rw-r--r--   0        0        0    13759 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/db_workbench.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/db_z_backend.py
--rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/menu.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/plugin_comments.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/processes.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/scheduler.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/tags.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/models/webtest_jwt_support.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/403.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/404.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/500.html
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/503.html
--rw-r--r--   0        0        0   128744 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/bootstrap.min.css
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/calendar.css
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/edit.css
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/master.css
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/web2py-bootstrap3.css
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/web2py.css
--rw-r--r--   0        0        0    90796 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/ProximaNovaLt.otf
--rw-r--r--   0        0        0    20127 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0   108738 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    45404 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23424 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0    18028 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0        0        0   740881 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/background.jpg
--rw-r--r--   0        0        0   165425 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/banner.ef18bff1.png
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/facebook.png
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/favicon.ico
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/favicon.png
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/gplus-32.png
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/twitter.png
--rw-r--r--   0        0        0   238247 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/analytics.min.js
--rw-r--r--   0        0        0    36816 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/bootstrap.min.js
--rw-r--r--   0        0        0    51765 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/calendar.js
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/edit.js
--rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/jquery.js
--rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/modernizr-2.8.3.min.js
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/respond-1.4.2.min.js
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/share.js
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/web2py-bootstrap3.js
--rw-r--r--   0        0        0    36093 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/web2py.js
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/__init__.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/appadmin.html
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.html
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.ics
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.jsonp
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.load
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.map
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.pdf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.rss
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.xml
--rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/layout.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/web2py_ajax.html
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/applog/applog_layout.html
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/applog/author.html
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/applog/index.html
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/applog/item.html
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/auto_tags.html
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/change_password.html
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/check_domeinen.html
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/domeinen.html
--rw-r--r--   0        0        0    18335 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/email_footer.html
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/email_footer_form.html
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/index.html
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/items.html
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/new_tag.html
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/overdragen.html
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/password_reset_are_you_sure.html
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/quick_create.html
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/quick_edit.html
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/sticker_beheer.html
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/tag_search.html
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/tag_search.load
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/taggem.html
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/user.html
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/users.html
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/organisations/boards.html
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/organisations/index.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/organisations/quick_create.html
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/organisations/quick_edit.html
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/apply_to_all.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/contacts.html
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/dod_rules.html
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/edit.html
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/index.html
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/item_dod_rules.html
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/item_questions.html
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/metadateren.html
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/new.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/questions.html
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/source_grid.load
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/tag.html
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/tag_beheer.html
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/tag_tree.load
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/.gitignore
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/LICENSE.txt
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/pyproject.toml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/readme.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 ontwikkelstraat-1.18.1/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/.dockerignore
+-rw-r--r--   0        0        0    54660 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/CHANGELOG.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/__init__.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/bundle-lts.yaml
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/bundle.yaml
+-rw-r--r--   0        0        0    20484 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docker-compose.yml
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/mkdocs.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/requirements.in
+-rw-r--r--   0        0        0    25604 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/tasks.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/architectuur-vanuit-netwerk-perspectief.md
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-installeer-je-omgevingen.md
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-testen-we-de-frontend.md
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-werken-verchillende-applicatie-versies.md
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-werken-we-met-branches.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-werken-we-met-ssh.md
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-werkt-de-backup-en-restore.md
+-rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-werkt-de-frontend.md
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-werkt-locust.md
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/hoe-wordt-een-server-geprovisioned.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/index.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/mkdocs.md
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/over-deze-documentatie.md
+-rw-r--r--   0        0        0    78735 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/playwright_img.png
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/sequence.puml
+-rw-r--r--   0        0        0   314339 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/versiebeheer-miro-bord.png
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-applog.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-celery.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-cmsx.md
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-de-bundler.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-de-feature-omgeving.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-de-fica-omgeving.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-de-workbench.md
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-docker-compose.md
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-docker.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-dotenv.md
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-een-omgeving.md
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-fabric.md
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-fragmentx.md
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-ghost.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-git.md
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-invoke.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-locust.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-lts.md
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-migrate.md
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-multipass.md
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-pip-compile.md
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-playwright.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-postgres.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-py4web.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-redis.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-restic.md
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-treafik.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-web2py.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-is-xonsh.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/docs/wat-zijn-de-core-libraries.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/requirements.in
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/requirements.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/.env.sample
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Ghost blog searcher.ipynb
+-rw-r--r--   0        0        0    30289 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Kladblaadje statistieken.ipynb
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Knutselwerk tags en items.ipynb
+-rw-r--r--   0        0        0   962690 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/LOF-ghost-archief.ipynb
+-rw-r--r--   0        0        0   103193 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Leids aanbod statistieken.ipynb
+-rw-r--r--   0        0        0    13322 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Nieuwe sticker toevoegen.ipynb
+-rw-r--r--   0        0        0    19551 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Regulier Tag Ondehoud.ipynb
+-rw-r--r--   0        0        0     9286 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Romy's database hoofd ontplof pagina.ipynb
+-rw-r--r--   0        0        0    44883 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Snippets en voorbeelden.ipynb
+-rw-r--r--   0        0        0   154863 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Tags and database tuning.ipynb
+-rw-r--r--   0        0        0    21225 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Widgets.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/__init__.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/__init__edwh__new.ipynb
+-rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/__init__edwh__notebooks.ipynb
+-rw-r--r--   0        0        0    41002 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/ghost.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/handig.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/item_search_quicky.ipynb
+-rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/nocodb.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/organisations_naar_changelog.ipynb
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/poging_plpython3.ipynb
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/quicky_tags_editen.ipynb
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/sqlite_to_pydal.ipynb
+-rw-r--r--   0        0        0   140777 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/ticket 248.ipynb
+-rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/DUO data importer - via API.ipynb
+-rw-r--r--   0        0        0    32676 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/DUO data importer - via datadump.ipynb
+-rw-r--r--   0        0        0    15029 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/Staging DUO data to effdted organisations.ipynb
+-rw-r--r--   0        0        0    68495 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/Untitled.ipynb
+-rw-r--r--   0        0        0    62640 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/scholenopdekaart data importer.ipynb
+-rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/views.sql
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/db/readme.md
+-rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/20230213 vo onderwijstype.ipynb
+-rw-r--r--   0        0        0    10759 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/21.11.25-Omgeving Leiden verhuizen.ipynb
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/IOL_import.ipynb
+-rw-r--r--   0        0        0   312854 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/Leids aanbod uit Ghost overzetten.ipynb
+-rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/Locatiegegevens aan Organisatie.ipynb
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/eddie-icon.png
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/opruimen_van_eddie_tags.ipynb
+-rw-r--r--   0        0        0    86596 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/qrcode demo.ipynb
+-rw-r--r--   0        0        0    45040 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/caching/caching-icm-shared-code.ipynb
+-rw-r--r--   0        0        0    40547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/caching/caching.ipynb
+-rw-r--r--   0        0        0    28437 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/sync/federation.ipynb
+-rw-r--r--   0        0        0    31541 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/jupyterlab/notebooks/sync/synchronize.ipynb
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/locust/docker-compose.yml
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/locust/locust_static_ghost.py
+-rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/locust/locustfile.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/migrate/Dockerfile
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/migrate/requirements.in
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/migrate/requirements.txt
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/migrate/data/README.md
+-rw-r--r--   0        0        0    67927 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/migrate/data/empty.sql
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/migrate/flags/README.txt
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/playwright_test/conftest.py
+-rw-r--r--   0        0        0    52511 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/playwright_test/test_static_ghost.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/playwright_test/screenshots/delete_all_screenshots.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/Dockerfile
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/py4web_bjoern.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/py4web_wsgi.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/requirements.in
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/requirements.txt
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/c/__init__.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/c/static/README.md
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/demo.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/fixtures.py
+-rw-r--r--   0        0        0    13812 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/handlebars.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/opengraph.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/settings.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/src/sass/main.scss
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/README.md
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/fonts.css
+-rw-r--r--   0        0        0  1497327 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/mystyles.css
+-rw-r--r--   0        0        0    62128 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/banner.webp
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/boy.png
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-by.svg
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-general.svg
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-nc-eu.svg
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-nd.svg
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-remix.svg
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-sa.svg
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-share.svg
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-zero.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/chevron-up.svg
+-rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/de-pionier.png
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/elders.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/email.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/grootte.svg
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/hier.svg
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/hs-leiden.png
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/icon.png
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/info.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/kennis.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/locatie.svg
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/logo.png
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/onderwijsniveau.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/onderwijstype.svg
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/pd.svg
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/pencil-solid.svg
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/profiel.svg
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/seal.png
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/user-solid.svg
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/users-solid.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/wetenschappelijk.svg
+-rw-r--r--   0        0        0   278644 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/_hyperscript_w9y-0.9.3.min.js
+-rw-r--r--   0        0        0   300008 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/_hyperscript_w9y-0.9.5-dev.min.js
+-rw-r--r--   0        0        0   290107 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/_hyperscript_w9y-dev.min.js
+-rw-r--r--   0        0        0   295499 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/_hyperscript_w9y.js
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/behaviors._hs
+-rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/browser-report.js
+-rw-r--r--   0        0        0    19796 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/bulma.js
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/commands._hs
+-rw-r--r--   0        0        0   129599 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/htmx.js
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/htmx_extend.js
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/javascript_dependencies.js
+-rw-r--r--   0        0        0    33273 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/leaflet-providers.js
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/activiteiten.hbs
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/attribution.hbs
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/component.hbs
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/demo.hbs
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/demo_component.hbs
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/demo_template.hbs
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/extern.hbs
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/hotspots.hbs
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/index.hbs
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/item.hbs
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/item.html
+-rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/leiden.hbs
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/loading-error.html
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/ratings.hbs
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/school.hbs
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/school.html
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/school_praktijkoverzicht.hbs
+-rw-r--r--   0        0        0    21455 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/template-item.html
+-rw-r--r--   0        0        0    26740 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/template.hbs
+-rw-r--r--   0        0        0    26702 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/template.html
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/template_minimal.hbs
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/user.hbs
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/user.html
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/__init__.py
+-rw-r--r--   0        0        0    23159 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/backend_support.py
+-rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/common.py
+-rw-r--r--   0        0        0    53219 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/controllers.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/fixtures.py
+-rw-r--r--   0        0        0    12261 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/handlebars.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/helpers.py
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/hotspots.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/models.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/requirements.txt
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/settings.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/tasks.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/databases/README.md
+-rw-r--r--   0        0        0  1050756 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/databases/plaatsen.json
+-rw-r--r--   0        0        0   812804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/databases/slugified_plaatsen.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/README.md
+-rw-r--r--   0        0        0  1750102 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/css/bundled-latest.css
+-rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/css/no.css
+-rw-r--r--   0        0        0    62128 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/banner.webp
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/boy.png
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-by.svg
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-general.svg
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-nc-eu.svg
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-nd.svg
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-remix.svg
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-sa.svg
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-share.svg
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-zero.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/chevron-up.svg
+-rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/de-pionier.png
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/elders.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/email.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/grootte.svg
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/hier.svg
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/hs-leiden.png
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/icon.png
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/info.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/kennis.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/locatie.svg
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/onderwijsniveau.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/onderwijstype.svg
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/pd.svg
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/pencil-solid.svg
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/profiel.svg
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/seal.png
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/user-solid.svg
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/users-solid.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/wetenschappelijk.svg
+-rw-r--r--   0        0        0    50592 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/a.png
+-rw-r--r--   0        0        0    32479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/b.png
+-rw-r--r--   0        0        0    52288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/c.png
+-rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/d.png
+-rw-r--r--   0        0        0    35976 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/e.png
+-rw-r--r--   0        0        0    15775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/f.png
+-rw-r--r--   0        0        0    42655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/g.png
+-rw-r--r--   0        0        0    26280 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/h.png
+-rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/i.png
+-rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/j.png
+-rw-r--r--   0        0        0    35274 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/k.png
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/l.png
+-rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/m.png
+-rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/n.png
+-rw-r--r--   0        0        0    27075 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/o.png
+-rw-r--r--   0        0        0    33183 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/p.png
+-rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/q.png
+-rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/r.png
+-rw-r--r--   0        0        0    46853 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/s.png
+-rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/t.png
+-rw-r--r--   0        0        0    21505 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/u.png
+-rw-r--r--   0        0        0    42804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/v.png
+-rw-r--r--   0        0        0    45793 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/w.png
+-rw-r--r--   0        0        0    29958 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/x.png
+-rw-r--r--   0        0        0    35670 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/y.png
+-rw-r--r--   0        0        0    23193 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/z.png
+-rw-r--r--   0        0        0   156808 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/js/bundled-latest.js
+-rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/js/utils.js
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/README.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/active-filters.hbs
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/active_filters.html
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth.html
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/component_loader.html
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/demo.hbs
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/external_tiles.hbs
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/external_tiles.html
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/filter-with-active.hbs
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/filter-with-active.html
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/filter.hbs
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/filter.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/generic.html
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/hotspots.hbs
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/hotspots.html
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/index.html
+-rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/item.hbs
+-rw-r--r--   0        0        0    42192 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/item.html
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/layout.html
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/list_items.hbs
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/menu.hbs
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/menu.html
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/modals.hbs
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/modals.html
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/notification.hbs
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/notification.html
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/page_header.hbs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/quick_filter.hbs
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/quick_filter.html
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/rating_form.hbs
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/rating_results.hbs
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/school.hbs
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/school.html
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/school_praktijkoverzicht.hbs
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/school_praktijkoverzicht.html
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/simple_analytics.html
+-rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/tiles.hbs
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/tiles.html
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/user.hbs
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/user.html
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/email_validate.hbs
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/email_validate.html
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/login.hbs
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/login.html
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/no_cookies.html
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/recover.hbs
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/recover.html
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/register1.hbs
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/register1.html
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/register2.hbs
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/register2.html
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/component/datalist_plaatsen.hbs
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/component/datalist_plaatsen.html
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/component/datalist_scholen.hbs
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/component/datalist_scholen.html
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filterbuttons.hbs
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filterbuttons.html
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filtermenu-modal.hbs
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filtermenu-modal.html
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filtermenu.hbs
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filtermenu.html
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/translations/empty.dir
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/translations/it.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/fragmentx/uploads/empty.dir
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/__init__.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/common.py
+-rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/controllers.py
+-rw-r--r--   0        0        0    12694 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/handlebars.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/helpers.py
+-rw-r--r--   0        0        0    32577 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/klassen_enquete.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/settings.py
+-rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/static/css/no.css
+-rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/static/js/utils.js
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/klassen_index.html
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/layout.html
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/enquete_uitslag.hbs
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/stapel.hbs
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/thema_uitleg.hbs
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/thema_uitleg_schoolleider.hbs
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/verdieping.hbs
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/vraag.hbs
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/demo.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/fixtures.py
+-rw-r--r--   0        0        0    13812 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/handlebars.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/opengraph.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/settings.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/src/sass/main.scss
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/README.md
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/fonts.css
+-rw-r--r--   0        0        0  1497263 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/mystyles.css
+-rw-r--r--   0        0        0    62128 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/banner.webp
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/boy.png
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/cc-by.svg
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/cc-general.svg
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/cc-sa.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/chevron-up.svg
+-rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/de-pionier.png
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/elders.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/email.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/grootte.svg
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/hier.svg
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/hs-leiden.png
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/info.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/kennis.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/locatie.svg
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/logo.png
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/onderwijsniveau.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/onderwijstype.svg
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/profiel.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/wetenschappelijk.svg
+-rw-r--r--   0        0        0   278644 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-0.9.3.min.js
+-rw-r--r--   0        0        0   300008 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-0.9.5-dev.min.js
+-rw-r--r--   0        0        0   290107 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-dev.min.js
+-rw-r--r--   0        0        0   295499 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/_hyperscript_w9y.js
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/behaviors._hs
+-rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/browser-report.js
+-rw-r--r--   0        0        0    19796 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/bulma.js
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/commands._hs
+-rw-r--r--   0        0        0   129599 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/htmx.js
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/htmx_extend.js
+-rw-r--r--   0        0        0    16194 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/javascript_dependencies.js
+-rw-r--r--   0        0        0    33273 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/leaflet-providers.js
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/activiteiten.hbs
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/attribution.hbs
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/component.hbs
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/demo.hbs
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/demo_component.hbs
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/demo_template.hbs
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/extern.hbs
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/hotspots.hbs
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/index.hbs
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/item.hbs
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/item.html
+-rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/leiden.hbs
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/loading-error.html
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/ratings.hbs
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/school.hbs
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/school.html
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/school_praktijkoverzicht.hbs
+-rw-r--r--   0        0        0    67801 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/template-item.html
+-rw-r--r--   0        0        0    90095 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/template.hbs
+-rw-r--r--   0        0        0    91770 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/template.html
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/template_minimal.hbs
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/user.hbs
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/user.html
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/jwt_demo/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/__init__.py
+-rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/common.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/controllers.py
+-rw-r--r--   0        0        0    41077 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/ghost.py
+-rw-r--r--   0        0        0    14685 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/handlebars.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/models.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/settings.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/tasks.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/databases/README.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/static/README.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/templates/index.hbs
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/__init__.py
+-rw-r--r--   0        0        0    23159 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/backend_support.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/common.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/common_lts.py
+-rw-r--r--   0        0        0    51846 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/controllers.py
+-rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/fixtures.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/fixtures_lts.py
+-rw-r--r--   0        0        0    19044 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/graphql_support.py
+-rw-r--r--   0        0        0    15020 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/handlebars.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/helpers.py
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/hotspots.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/klassen_controllers.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/klassen_enquete.py
+-rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/lts_controllers.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/markdown_template.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/models.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/models_lts.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/requirements.txt
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/settings.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/tasks.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/databases/README.md
+-rw-r--r--   0        0        0  5011320 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/databases/lts_assets.sql
+-rw-r--r--   0        0        0  1050756 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/databases/plaatsen.json
+-rw-r--r--   0        0        0   812804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/databases/slugified_plaatsen.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/README.md
+-rw-r--r--   0        0        0  1750102 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/css/bundled-1.0.0.css
+-rw-r--r--   0        0        0  1748035 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/css/bundled.css
+-rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/css/no.css
+-rw-r--r--   0        0        0    62128 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/banner.webp
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/boy.png
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-by.svg
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-general.svg
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-nc-eu.svg
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-nd.svg
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-remix.svg
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-sa.svg
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-share.svg
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-zero.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/chevron-up.svg
+-rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/de-pionier.png
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/elders.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/email.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/grootte.svg
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/hier.svg
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/hs-leiden.png
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/icon.png
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/info.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/kennis.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/locatie.svg
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/onderwijsniveau.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/onderwijstype.svg
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/pd.svg
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/pencil-solid.svg
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/profiel.svg
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/seal.png
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/user-solid.svg
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/users-solid.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/wetenschappelijk.svg
+-rw-r--r--   0        0        0    50592 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/a.png
+-rw-r--r--   0        0        0    32479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/b.png
+-rw-r--r--   0        0        0    52288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/c.png
+-rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/d.png
+-rw-r--r--   0        0        0    35976 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/e.png
+-rw-r--r--   0        0        0    15775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/f.png
+-rw-r--r--   0        0        0    42655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/g.png
+-rw-r--r--   0        0        0    26280 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/h.png
+-rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/i.png
+-rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/j.png
+-rw-r--r--   0        0        0    35274 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/k.png
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/l.png
+-rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/m.png
+-rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/n.png
+-rw-r--r--   0        0        0    27075 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/o.png
+-rw-r--r--   0        0        0    33183 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/p.png
+-rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/q.png
+-rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/r.png
+-rw-r--r--   0        0        0    46853 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/s.png
+-rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/t.png
+-rw-r--r--   0        0        0    21505 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/u.png
+-rw-r--r--   0        0        0    42804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/v.png
+-rw-r--r--   0        0        0    45793 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/w.png
+-rw-r--r--   0        0        0    29958 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/x.png
+-rw-r--r--   0        0        0    35670 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/y.png
+-rw-r--r--   0        0        0    23193 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/z.png
+-rw-r--r--   0        0        0   156294 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/js/bundled-1.0.0.js
+-rw-r--r--   0        0        0   156483 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/js/bundled.js
+-rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/static/js/utils.js
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/README.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/active-filters.hbs
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/active_filters.html
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth.html
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/changelog.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component_loader.html
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/demo.hbs
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/documentatie.md
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/email_registration_form.hbs
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/email_registration_form.html
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/enquete_uitslag.hbs
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/external_tiles.hbs
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/external_tiles.html
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/filter-with-active.hbs
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/filter-with-active.html
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/filter.hbs
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/filter.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/generic.html
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/hotspots.hbs
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/hotspots.html
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/index.html
+-rw-r--r--   0        0        0    28247 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/item.hbs
+-rw-r--r--   0        0        0    32978 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/item.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/klassen_index.html
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/layout.html
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/list_items.hbs
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/menu.hbs
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/menu.html
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/modals.hbs
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/modals.html
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/notification.hbs
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/notification.html
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/page_header.hbs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/quick_filter.hbs
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/quick_filter.html
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/rating_form.hbs
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/rating_results.hbs
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/school.hbs
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/school.html
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/school_praktijkoverzicht.hbs
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/school_praktijkoverzicht.html
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/stapel.hbs
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/thema_uitleg.hbs
+-rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/tiles.hbs
+-rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/tiles.html
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/user.hbs
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/user.html
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/vraag.hbs
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/email_validate.hbs
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/email_validate.html
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/login.hbs
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/login.html
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/recover.hbs
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/recover.html
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/register1.hbs
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/register1.html
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/register2.hbs
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/register2.html
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/danger.hbs
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/danger.html
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/datalist_plaatsen.hbs
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/datalist_plaatsen.html
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/datalist_scholen.hbs
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/datalist_scholen.html
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/success.hbs
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/success.html
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/warning.hbs
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/component/warning.html
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/layouts/generic.hbs
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/layouts/markdown.html
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_1.html
+-rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_2.html
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_3.html
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_layout.html
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_tags.html
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/demo.html
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/demo_template.html
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/manage.html
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/manage_grid.html
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/manage_groups.html
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filterbuttons.hbs
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filterbuttons.html
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filtermenu-modal.hbs
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filtermenu-modal.html
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filtermenu.hbs
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filtermenu.html
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/translations/empty.dir
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/translations/it.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/lts/uploads/empty.dir
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/__init__.py
+-rw-r--r--   0        0        0    23159 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/backend_support.py
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/common.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/controllers.py
+-rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/fixtures.py
+-rw-r--r--   0        0        0    12261 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/handlebars.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/helpers.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/requirements.txt
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/settings.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/tasks.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/databases/README.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/README.md
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/LEF logo.svg
+-rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/Onderwijsindeleidseregio logo.svg
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/icon.png
+-rw-r--r--   0        0        0    50592 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/a.png
+-rw-r--r--   0        0        0    32479 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/b.png
+-rw-r--r--   0        0        0    52288 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/c.png
+-rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/d.png
+-rw-r--r--   0        0        0    35976 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/e.png
+-rw-r--r--   0        0        0    15775 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/f.png
+-rw-r--r--   0        0        0    42655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/g.png
+-rw-r--r--   0        0        0    26280 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/h.png
+-rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/i.png
+-rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/j.png
+-rw-r--r--   0        0        0    35274 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/k.png
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/l.png
+-rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/m.png
+-rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/n.png
+-rw-r--r--   0        0        0    27075 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/o.png
+-rw-r--r--   0        0        0    33183 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/p.png
+-rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/q.png
+-rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/r.png
+-rw-r--r--   0        0        0    46853 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/s.png
+-rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/t.png
+-rw-r--r--   0        0        0    21505 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/u.png
+-rw-r--r--   0        0        0    42804 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/v.png
+-rw-r--r--   0        0        0    45793 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/w.png
+-rw-r--r--   0        0        0    29958 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/x.png
+-rw-r--r--   0        0        0    35670 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/y.png
+-rw-r--r--   0        0        0    23193 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/z.png
+-rw-r--r--   0        0        0     8763 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/templates/narrowcasting.html
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/translations/empty.dir
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/translations/it.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/uploads/empty.dir
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/restart/__init__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/restart/static/README.md
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/restart/static/favicon.ico
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/__init__.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/common.py
+-rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/controllers.py
+-rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/handlebars.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/models.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/settings.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/tasks.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/databases/README.md
+-rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/databases/dna.csv
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/static/README.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/card.hbs
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/ghost.hbs
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/index.hbs
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/uitslag.hbs
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/vraag.hbs
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/py4web/uploaded_attachments/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/__init__.py
+-rw-r--r--   0        0        0    30942 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/data_model.py
+-rw-r--r--   0        0        0    69719 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/migrations.py
+-rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/tags.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/asink.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/celerysink.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/diskcachesink.py
+-rw-r--r--   0        0        0    14089 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/signalemitter.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/sink.py
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/tasks.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/__init__.py
+-rw-r--r--   0        0        0    94817 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/engine.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/ntfy_sh.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/opengraph.py
+-rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/support.py
+-rw-r--r--   0        0        0    21771 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/tasks.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/jwt_tools/__init__.py
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/jwt_tools/jwt_py4web.py
+-rw-r--r--   0        0        0     6934 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/jwt_tools/jwt_web2py.py
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/jwt_tools/shared.py
+-rw-r--r--   0        0        0    18276 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/pgcache/__init__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/pgcache/clean.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/pgcache/define_models.py
+-rw-r--r--   0        0        0     8712 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/sync/__init__.py
+-rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/shared_code/edwh/core/web2py_tools/__init__.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/Dockerfile
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/requirements.in
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/requirements.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/routes.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/readme.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/ABOUT
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/LICENSE
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/progress.log
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/routes.example.py
+-rw-r--r--   0        0        0    27197 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/controllers/appadmin.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/controllers/default.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/cron/crontab
+-rw-r--r--   0        0        0    16269 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/ar.py
+-rw-r--r--   0        0        0    15922 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/ca.py
+-rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/cs.py
+-rw-r--r--   0        0        0    16378 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/de.py
+-rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/en.py
+-rw-r--r--   0        0        0    16113 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/es.py
+-rw-r--r--   0        0        0    15937 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/fr-ca.py
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/fr.py
+-rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/hi.py
+-rw-r--r--   0        0        0    15342 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/hu.py
+-rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/id.py
+-rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/it.py
+-rw-r--r--   0        0        0    19085 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/my-mm.py
+-rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/my.py
+-rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/nl.py
+-rw-r--r--   0        0        0    15452 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/pl.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/plural-cs.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/plural-en.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/plural-es.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/plural-ru.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/plural-uk.py
+-rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/pt-br.py
+-rw-r--r--   0        0        0    15449 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/pt.py
+-rw-r--r--   0        0        0    15584 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/ro.py
+-rw-r--r--   0        0        0    16418 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/ru.py
+-rw-r--r--   0        0        0    15548 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/sk.py
+-rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/tr.py
+-rw-r--r--   0        0        0    18665 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/uk.py
+-rw-r--r--   0        0        0    15285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/zh-cn.py
+-rw-r--r--   0        0        0    15437 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/zh-tw.py
+-rw-r--r--   0        0        0    15437 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/zh.py
+-rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/models/db.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/models/menu.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/modules/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/private/appconfig.ini
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/403.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/404.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/500.html
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/503.html
+-rw-r--r--   0        0        0   144877 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   551641 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/calendar.css
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/web2py-bootstrap4.css
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/web2py.css
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/images/facebook.png
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/images/favicon.ico
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/images/favicon.png
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/images/gplus-32.png
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/images/twitter.png
+-rw-r--r--   0        0        0   238247 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/analytics.min.js
+-rw-r--r--   0        0        0    67742 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   273872 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0    51765 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/calendar.js
+-rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/jquery.js
+-rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/modernizr-2.8.3.min.js
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/web2py-bootstrap4.js
+-rw-r--r--   0        0        0    37138 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/web2py.js
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/__init__.py
+-rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/appadmin.html
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.csv
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.html
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.ics
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.jsonp
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.load
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.map
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.pdf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.rss
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.xml
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/layout.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/web2py_ajax.html
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/default/index.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/default/netwerken.html
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/default/socialmedia.html
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/default/user.html
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/.gitignore
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/ABOUT
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/LICENSE
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/__init__.py
+-rw-r--r--   0        0        0   743011 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/errors.tgz
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/progress.log
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/requirements.txt
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/routes.example.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/api.py
+-rw-r--r--   0        0        0    26987 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/appadmin.py
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/applog.py
+-rw-r--r--   0        0        0    63924 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/default.py
+-rw-r--r--   0        0        0    27300 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/dv_appadmin.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/jwt_auth.py
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/organisations.py
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/plugin_comments.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/scratch.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/webtest_support.py
+-rw-r--r--   0        0        0    33810 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/workbench.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/cron/crontab
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/cron/crontab.example
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_apply_to_all_items.table
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_contact.table
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_dod_rule.table
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item.table
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_dod_rule.table
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_question.table
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_tag.table
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_plugin_comments_comment.table
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_question.table
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_source_file.table
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_tag_dod_rule.table
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_tag_question.table
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_cas.table
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_event.table
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_group.table
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_permission.table
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_run.table
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_task.table
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_task_deps.table
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_worker.table
+-rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/sql.log
+-rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/storage.sqlite
+-rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/workbench.sqlite
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/functional_test/readme.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/functional_test/requirements.txt
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/functional_test/test.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/functional_test/tools.py
+-rw-r--r--   0        0        0    27990 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/ca.py
+-rw-r--r--   0        0        0    27762 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/cs.py
+-rw-r--r--   0        0        0    11394 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/de.py
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/en.py
+-rw-r--r--   0        0        0    25538 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/es.py
+-rw-r--r--   0        0        0    12596 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/fr-ca.py
+-rw-r--r--   0        0        0    12483 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/fr.py
+-rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/hi.py
+-rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/hu.py
+-rw-r--r--   0        0        0    17432 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/id.py
+-rw-r--r--   0        0        0    13544 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/it.py
+-rw-r--r--   0        0        0    19957 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/my-mm.py
+-rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/my.py
+-rw-r--r--   0        0        0    29472 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/nl.py
+-rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/pl.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/plural-cs.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/plural-en.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/plural-es.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/plural-ru.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/plural-uk.py
+-rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/pt-br.py
+-rw-r--r--   0        0        0    10738 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/pt.py
+-rw-r--r--   0        0        0    21571 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/ro.py
+-rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/ru.py
+-rw-r--r--   0        0        0    10469 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/sk.py
+-rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/tr.py
+-rw-r--r--   0        0        0    17857 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/uk.py
+-rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/zh-cn.py
+-rw-r--r--   0        0        0    14367 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/zh-tw.py
+-rw-r--r--   0        0        0    13777 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/zh.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/aaa_400_better_error_messages.py
+-rw-r--r--   0        0        0    16353 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/aaa_500_checkbox_widget.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/article_importers.py
+-rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/db.py
+-rw-r--r--   0        0        0    13759 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/db_workbench.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/db_z_backend.py
+-rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/menu.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/plugin_comments.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/processes.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/scheduler.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/tags.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/models/webtest_jwt_support.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/403.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/404.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/500.html
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/503.html
+-rw-r--r--   0        0        0   128744 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/calendar.css
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/edit.css
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/master.css
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/web2py-bootstrap3.css
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/web2py.css
+-rw-r--r--   0        0        0    90796 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/ProximaNovaLt.otf
+-rw-r--r--   0        0        0    20127 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0   108738 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    45404 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23424 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0   740881 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/background.jpg
+-rw-r--r--   0        0        0   165425 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/banner.ef18bff1.png
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/facebook.png
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/favicon.ico
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/favicon.png
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/gplus-32.png
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/twitter.png
+-rw-r--r--   0        0        0   238247 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/analytics.min.js
+-rw-r--r--   0        0        0    36816 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0    51765 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/calendar.js
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/edit.js
+-rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/jquery.js
+-rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/modernizr-2.8.3.min.js
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/respond-1.4.2.min.js
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/share.js
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/web2py-bootstrap3.js
+-rw-r--r--   0        0        0    36093 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/web2py.js
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/__init__.py
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/appadmin.html
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.html
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.ics
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.jsonp
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.load
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.map
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.pdf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.rss
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.xml
+-rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/layout.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/web2py_ajax.html
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/applog/applog_layout.html
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/applog/author.html
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/applog/index.html
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/applog/item.html
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/auto_tags.html
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/change_password.html
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/check_domeinen.html
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/domeinen.html
+-rw-r--r--   0        0        0    18335 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/email_footer.html
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/email_footer_form.html
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/index.html
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/items.html
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/new_tag.html
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/overdragen.html
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/password_reset_are_you_sure.html
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/quick_create.html
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/quick_edit.html
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/sticker_beheer.html
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/tag_search.html
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/tag_search.load
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/taggem.html
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/user.html
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/users.html
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/organisations/boards.html
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/organisations/index.html
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/organisations/quick_create.html
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/organisations/quick_edit.html
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/apply_to_all.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/contacts.html
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/dod_rules.html
+-rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/edit.html
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/index.html
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/item_dod_rules.html
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/item_questions.html
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/metadateren.html
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/new.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/questions.html
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/source_grid.load
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/tag.html
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/tag_beheer.html
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/tag_tree.load
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/.gitignore
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/LICENSE.txt
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/readme.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 ontwikkelstraat-1.19.0/PKG-INFO
```

### Comparing `ontwikkelstraat-1.18.1/CHANGELOG.md` & `ontwikkelstraat-1.19.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,59 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.19.0 (2024-04-18)
+
+### Feature
+
+* Add address to coordinates conversion feature ([`4456593`](https://github.com/educationwarehouse/ontwikkelstraat/commit/4456593da89d1d41730714f4fafe378ac18a852f))
+
+### Fix
+
+* Pip.compile web2py requirements because geopy was added to .in + refactor `load_geo` code ([`83b8e5e`](https://github.com/educationwarehouse/ontwikkelstraat/commit/83b8e5ecf2d80a203553bfd2719d6a35bde8fd83))
+* Nominatim er weer uit gesloopt ([`6384a34`](https://github.com/educationwarehouse/ontwikkelstraat/commit/6384a34948fc90eb9ee6dad6aa4bc8f93ccad663))
+
+## v1.18.6 (2024-04-11)
+
+### Fix
+
+* **tags:** Use request.args instead of request.vars ([`2d45532`](https://github.com/educationwarehouse/ontwikkelstraat/commit/2d455323d8627c2d8c5fb5963223cf07568d4935))
+
+## v1.18.5 (2024-04-11)
+
+### Fix
+
+* **tag:** Workbench tag page should also work via args (instead of just vars) ([`c167de5`](https://github.com/educationwarehouse/ontwikkelstraat/commit/c167de549f4dd3fb78eeb54c8b63c9877dcbb6d8))
+
+## v1.18.4 (2024-04-11)
+
+### Fix
+
+* **autotag:** Edit_tag/<gid> page does not exist, it should be workbench/tag/<gid> ([`babd5b7`](https://github.com/educationwarehouse/ontwikkelstraat/commit/babd5b788009b782df0886ca3949f0e59b09a033))
+
+## v1.18.3 (2024-04-11)
+
+### Fix
+
+* '.name' still doesn't exist on None ([`e63c657`](https://github.com/educationwarehouse/ontwikkelstraat/commit/e63c657bf7198bcabeb1eb99ac5b1d2860ebf0f6))
+
+## v1.18.2 (2024-04-11)
+
+### Fix
+
+* Bump dependencies again because certbot found another ([`ad51550`](https://github.com/educationwarehouse/ontwikkelstraat/commit/ad515504825501d7bfdc3bb239915ddc5b00ce5f))
+* Additional fix for 'Tagged In Db' removed tags ([`0ec7d6d`](https://github.com/educationwarehouse/ontwikkelstraat/commit/0ec7d6d63b8295c1825d0ecac198def544a98ee1))
+* Auto tag for missing gid should not crash the whole autotag page ([`a5e54e9`](https://github.com/educationwarehouse/ontwikkelstraat/commit/a5e54e9e5e43431a430784a6ecc239238822c4cb))
+
+### Performance
+
+* Speed up docker builds by doing COPY as late as possible (-> can cache more steps) ([`dfd5c3a`](https://github.com/educationwarehouse/ontwikkelstraat/commit/dfd5c3aa84d1f416d1732a649d6679c507094003))
+* **docker:** Installeer eerst web2py en dan de andere dependencies. Dan is rebuild sneller (want w2p install is gecached) ([`0f5de90`](https://github.com/educationwarehouse/ontwikkelstraat/commit/0f5de9000a289b2e2a04f9ee5a8fbdd61372692d))
+
 ## v1.18.1 (2024-03-21)
 
 ### Fix
 
 * Bump dependencies (make dependabot happy) ([`21b9a27`](https://github.com/educationwarehouse/ontwikkelstraat/commit/21b9a2784d6b01c34efd73719bca0d8adec3248f))
 * **sticker_link:** Added xml ([`d443b61`](https://github.com/educationwarehouse/ontwikkelstraat/commit/d443b61dbab4bda1e644567091579bef3c425758))
 * **stickers:** Web2py sticker beheer - gebruik nieuwe htmx widget + cleanup code ([`70edf50`](https://github.com/educationwarehouse/ontwikkelstraat/commit/70edf50b63a617bfdc7526c96ac95a9a6ab6447f))
```

### Comparing `ontwikkelstraat-1.18.1/bundle-lts.yaml` & `ontwikkelstraat-1.19.0/bundle-lts.yaml`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/bundle.yaml` & `ontwikkelstraat-1.19.0/bundle.yaml`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docker-compose.yml` & `ontwikkelstraat-1.19.0/docker-compose.yml`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 
   pgpool: # reverse proxy and switcher. partly works
     hostname: pgpool
     image: bitnami/pgpool:4.3.1
     ports:
       - "${PGPOOL_PORT}:5432"
     environment:
-      - PGPOOL_BACKEND_NODES=0:pg-0:5432 #, 1:pg-1:5432
+      - PGPOOL_BACKEND_NODES=0:pg-0:5432,1:pg-1:5432
       - PGPOOL_SR_CHECK_USER=postgres
       - PGPOOL_SR_CHECK_PASSWORD=password
       - PGPOOL_ENABLE_LDAP=no
       - PGPOOL_POSTGRES_USERNAME=postgres
       - PGPOOL_POSTGRES_PASSWORD=password
       - PGPOOL_ADMIN_USERNAME=postgres
       - PGPOOL_ADMIN_PASSWORD=password
@@ -467,15 +467,15 @@
       - PGPOOL_ENABLE_LOG_CONNECTIONS=no
       # - PGPOOL_ENABLE_LOG_PER_NODE_STATEMENT=no
       - PGPOOL_SERIALIZE_ACCEPT=on #  When set to on, Pgpool-II enables the serialization on incoming client connections. Without serialization the OS kernel wakes up all of the Pgpool-II children processes to execute accept() and one of them actually gets the incoming connection. The problem here is, because so my child process wake up at a same time, heavy context switching occurs and the performance is affected.
       - PGPOOL_RESERVED_CONNECTIONS=1 #   When this parameter is set to 1 or greater, incoming connections from clients are not accepted with error message "Sorry, too many clients already", rather than blocked if the number of current connections from clients is more than (num_init_children - reserved_connections). For example, if reserved_connections = 1 and num_init_children = 32, then the 32th connection from a client will be refused. This behavior is similar to PostgreSQL and good for systems on which the number of connections from clients is large and each session may take long time. In this case length of the listen queue could be very long and may cause the system unstable. In this situation setting this parameter to non 0 is a good idea to prevent the listen queue becomes very long.
       - PGPOOL_AUTHENTICATION_METHOD=scram-sha-256
     depends_on:
       - pg-0
-    # - pg-1
+      - pg-1
     networks:
       backend:
         aliases:
           - pgpool
     logging:
       driver: "json-file"
       options:
@@ -534,14 +534,15 @@
           - pg-1
     logging:
       driver: "json-file"
       options:
         max-size: "25m"
         max-file: "2"
 
+
 ######## we love these guys
 # prune old ones once in while with "docker volume prune",
 # WARNING WARNING: ONLY WHEN YOU HAVE RUNNING INSTANCES WITH PRODUCTION DATA
 # otherwise EVERYTHING will be whiped.
 #
 volumes:
   pg_0_data:
```

### Comparing `ontwikkelstraat-1.18.1/mkdocs.yml` & `ontwikkelstraat-1.19.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/tasks.py` & `ontwikkelstraat-1.19.0/tasks.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/architectuur-vanuit-netwerk-perspectief.md` & `ontwikkelstraat-1.19.0/docs/architectuur-vanuit-netwerk-perspectief.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/hoe-installeer-je-omgevingen.md` & `ontwikkelstraat-1.19.0/docs/hoe-installeer-je-omgevingen.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/hoe-testen-we-de-frontend.md` & `ontwikkelstraat-1.19.0/docs/hoe-testen-we-de-frontend.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/hoe-werken-verchillende-applicatie-versies.md` & `ontwikkelstraat-1.19.0/docs/hoe-werken-verchillende-applicatie-versies.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/hoe-werken-we-met-branches.md` & `ontwikkelstraat-1.19.0/docs/hoe-werken-we-met-branches.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/hoe-werkt-de-backup-en-restore.md` & `ontwikkelstraat-1.19.0/docs/hoe-werkt-de-backup-en-restore.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/hoe-werkt-de-frontend.md` & `ontwikkelstraat-1.19.0/docs/hoe-werkt-de-frontend.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/hoe-werkt-locust.md` & `ontwikkelstraat-1.19.0/docs/hoe-werkt-locust.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/index.md` & `ontwikkelstraat-1.19.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/mkdocs.md` & `ontwikkelstraat-1.19.0/docs/mkdocs.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/over-deze-documentatie.md` & `ontwikkelstraat-1.19.0/docs/over-deze-documentatie.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/playwright_img.png` & `ontwikkelstraat-1.19.0/docs/playwright_img.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/sequence.puml` & `ontwikkelstraat-1.19.0/docs/sequence.puml`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/versiebeheer-miro-bord.png` & `ontwikkelstraat-1.19.0/docs/versiebeheer-miro-bord.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-applog.md` & `ontwikkelstraat-1.19.0/docs/wat-is-applog.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-de-bundler.md` & `ontwikkelstraat-1.19.0/docs/wat-is-de-bundler.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-docker-compose.md` & `ontwikkelstraat-1.19.0/docs/wat-is-docker-compose.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-docker.md` & `ontwikkelstraat-1.19.0/docs/wat-is-docker.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-een-omgeving.md` & `ontwikkelstraat-1.19.0/docs/wat-is-een-omgeving.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-fabric.md` & `ontwikkelstraat-1.19.0/docs/wat-is-fabric.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-ghost.md` & `ontwikkelstraat-1.19.0/docs/wat-is-ghost.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-git.md` & `ontwikkelstraat-1.19.0/docs/wat-is-git.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-invoke.md` & `ontwikkelstraat-1.19.0/docs/wat-is-invoke.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-locust.md` & `ontwikkelstraat-1.19.0/docs/wat-is-locust.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-lts.md` & `ontwikkelstraat-1.19.0/docs/wat-is-lts.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-migrate.md` & `ontwikkelstraat-1.19.0/docs/wat-is-migrate.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-multipass.md` & `ontwikkelstraat-1.19.0/docs/wat-is-multipass.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-pip-compile.md` & `ontwikkelstraat-1.19.0/docs/wat-is-pip-compile.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-playwright.md` & `ontwikkelstraat-1.19.0/docs/wat-is-playwright.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-py4web.md` & `ontwikkelstraat-1.19.0/docs/wat-is-py4web.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/docs/wat-is-restic.md` & `ontwikkelstraat-1.19.0/docs/wat-is-restic.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/Dockerfile` & `ontwikkelstraat-1.19.0/jupyterlab/Dockerfile`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/requirements.in` & `ontwikkelstraat-1.19.0/jupyterlab/requirements.in`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/requirements.txt` & `ontwikkelstraat-1.19.0/jupyterlab/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile jupyterlab/requirements.in --output-file jupyterlab/requirements.txt
+#    uv pip compile jupyterlab/requirements.in --output-file jupyterlab/requirements.txt --upgrade
 amqp==5.2.0
     # via kombu
 ansi==0.3.7
     # via edwh
 anyio==4.3.0
     # via
     #   httpx
@@ -16,23 +16,21 @@
     # via argon2-cffi
 arrow==1.3.0
     # via
     #   b2
     #   isoduration
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via redis
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-b2==3.17.0
+b2==3.18.0
     # via edwh-b2-plugin
-b2sdk==1.33.0
+b2sdk==2.0.0
     # via b2
 bcrypt==4.1.2
     # via paramiko
 beautifulsoup4==4.12.3
     # via nbconvert
 billiard==4.2.0
     # via celery
@@ -55,15 +53,15 @@
 click==8.1.7
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   edwh
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
 configuraptor==1.26.2
     # via
@@ -83,15 +81,15 @@
     # via fabric
 diceware==0.10
     # via
     #   edwh
     #   edwh-restic-plugin
 dill==0.3.8
 diskcache==5.6.3
-docutils==0.20.1
+docutils==0.21.1
     # via b2
 edwh==0.40.3
     # via
     #   edwh-pipcompile-plugin
     #   edwh-restic-plugin
     #   edwh-server-provisioning-plugin
     #   edwh-uptime-plugin
@@ -118,46 +116,42 @@
     # via edwh
 edwh-server-provisioning-plugin==0.4.7
     # via edwh
 edwh-sshfs-plugin==0.1.5
     # via edwh
 edwh-sshkey-plugin==0.1.7
     # via edwh
-edwh-uptime-plugin==0.3.4
+edwh-uptime-plugin==0.3.5
     # via edwh
 edwh-whitelabel-plugin==0.1.1
     # via edwh
-exceptiongroup==1.2.0
-    # via
-    #   anyio
-    #   ipython
 executing==2.0.1
     # via stack-data
 fabric==3.2.2
     # via
     #   edwh
     #   edwh-server-provisioning-plugin
     #   edwh-sshfs-plugin
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
 fqdn==1.5.1
     # via jsonschema
 greenlet==3.0.3
     # via sqlalchemy
 h11==0.14.0
     # via httpcore
-httpcore==1.0.4
+httpcore==1.0.5
     # via httpx
 httpx==0.27.0
 humanize==4.9.0
     # via
     #   edwh
     #   edwh-b2-plugin
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   httpx
     #   jsonschema
     #   requests
     #   yarl
     #   yayarl
@@ -168,15 +162,15 @@
     #   edwh-bundler-plugin
     #   edwh-demo-plugin
     #   edwh-locust-plugin
     #   edwh-multipass-plugin
     #   edwh-restic-plugin
     #   edwh-sshkey-plugin
     #   fabric
-ipython==8.22.2
+ipython==8.23.0
     # via ipython-sql
 ipython-genutils==0.2.0
     # via ipython-sql
 ipython-sql==0.5.0
 iso3166==2.1.1
 isoduration==20.11.0
     # via jsonschema
@@ -207,18 +201,18 @@
     #   nbformat
 jupyter-events==0.10.0
     # via jupyter-server
 jupyter-server==2.13.0
     # via jupyterlab-myst
 jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab-myst==2.3.1
+jupyterlab-myst==2.3.2
 jupyterlab-pygments==0.3.0
     # via nbconvert
-kombu==5.3.5
+kombu==5.3.6
     # via celery
 libsass==0.23.0
     # via edwh-bundler-plugin
 logfury==1.0.1
     # via b2sdk
 markdown-it-py==3.0.0
     # via rich
@@ -236,39 +230,38 @@
 more-itertools==10.2.0
 multidict==6.0.5
     # via
     #   yarl
     #   yayarl
 nbclient==0.10.0
     # via nbconvert
-nbconvert==7.16.2
+nbconvert==7.16.3
     # via jupyter-server
-nbformat==5.10.3
+nbformat==5.10.4
     # via
     #   jupyter-server
     #   nbclient
     #   nbconvert
 numpy==1.26.4
     # via pandas
 overrides==7.7.0
     # via jupyter-server
 packaging==24.0
     # via
-    #   b2sdk
     #   edwh
     #   jupyter-server
     #   nbconvert
-pandas==2.2.1
+pandas==2.2.2
 pandocfilters==1.5.1
     # via nbconvert
 paramiko==3.4.0
     # via
     #   fabric
     #   sshtunnel
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 phx-class-registry==4.1.0
     # via b2
 platformdirs==4.2.0
     # via
@@ -295,15 +288,15 @@
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
 pybars4==0.9.13
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pydal==20231114.3
     # via edwh-migrate
 pygments==2.17.2
     # via
     #   ipython
     #   nbconvert
@@ -338,15 +331,15 @@
     #   edwh-bundler-plugin
     #   edwh-server-provisioning-plugin
     #   jupyter-events
 pyzmq==25.1.2
     # via
     #   jupyter-client
     #   jupyter-server
-rapidfuzz==3.6.2
+rapidfuzz==3.8.1
     # via edwh
 redis==5.0.3
     # via edwh-migrate
 referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
@@ -374,15 +367,15 @@
     # via edwh-bundler-plugin
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
 rst2ansi==0.1.5
     # via b2
-send2trash==1.8.2
+send2trash==1.8.3
     # via jupyter-server
 setuptools==69.2.0
     # via diceware
 six==1.16.0
     # via
     #   asttokens
     #   bleach
@@ -391,15 +384,15 @@
     #   rfc3339-validator
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
 soupsieve==2.5
     # via beautifulsoup4
-sqlalchemy==2.0.28
+sqlalchemy==2.0.29
     # via ipython-sql
 sqlparse==0.4.4
     # via ipython-sql
 sshtunnel==0.4.0
 stack-data==0.6.3
     # via ipython
 tabulate==0.9.0
@@ -421,63 +414,65 @@
 tinycss2==1.2.1
     # via nbconvert
 tomli==2.0.1
     # via
     #   configuraptor
     #   edwh-pipcompile-plugin
 tomli-w==1.0.0
-    # via configuraptor
+    # via
+    #   configuraptor
+    #   edwh-uptime-plugin
 tomlkit==0.12.4
     # via edwh
 tornado==6.4
     # via
     #   jupyter-client
     #   jupyter-server
     #   terminado
 tqdm==4.66.2
     # via
     #   b2
-    #   b2sdk
     #   edwh-restic-plugin
 traitlets==5.14.2
     # via
     #   ipython
     #   jupyter-client
     #   jupyter-core
     #   jupyter-events
     #   jupyter-server
     #   matplotlib-inline
     #   nbclient
     #   nbconvert
     #   nbformat
-typeguard==4.1.5
+typeguard==4.2.1
     # via configuraptor
 types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
-    #   anyio
     #   b2sdk
     #   configuraptor
     #   edwh-pipcompile-plugin
     #   edwh-restic-plugin
+    #   edwh-uptime-plugin
+    #   ipython
     #   sqlalchemy
     #   typeguard
 tzdata==2024.1
     # via
     #   celery
     #   pandas
 ua-parser==0.18.0
     # via user-agents
 uri-template==1.3.0
     # via jsonschema
 urllib3==2.2.1
     # via requests
 user-agents==2.2.0
-uv==0.1.23
+uv==0.1.31
     # via
     #   edwh
     #   edwh-pipcompile-plugin
 vine==5.1.0
     # via
     #   amqp
     #   celery
```

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Ghost blog searcher.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Ghost blog searcher.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Kladblaadje statistieken.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Kladblaadje statistieken.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Knutselwerk tags en items.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Knutselwerk tags en items.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/LOF-ghost-archief.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/LOF-ghost-archief.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Leids aanbod statistieken.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Leids aanbod statistieken.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Nieuwe sticker toevoegen.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Nieuwe sticker toevoegen.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Regulier Tag Ondehoud.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Regulier Tag Ondehoud.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Romy's database hoofd ontplof pagina.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Romy's database hoofd ontplof pagina.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Snippets en voorbeelden.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Snippets en voorbeelden.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Tags and database tuning.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Tags and database tuning.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Widgets.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Widgets.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/__init__edwh__new.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/__init__edwh__new.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/__init__edwh__notebooks.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/__init__edwh__notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/ghost.py` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/ghost.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/handig.py` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/handig.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/item_search_quicky.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/item_search_quicky.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/nocodb.py` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/nocodb.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/organisations_naar_changelog.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/organisations_naar_changelog.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/poging_plpython3.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/poging_plpython3.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/quicky_tags_editen.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/quicky_tags_editen.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/sqlite_to_pydal.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/sqlite_to_pydal.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/ticket 248.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/ticket 248.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/DUO data importer - via API.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/DUO data importer - via API.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/DUO data importer - via datadump.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/DUO data importer - via datadump.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/Staging DUO data to effdted organisations.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/Staging DUO data to effdted organisations.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/Untitled.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/scholenopdekaart data importer.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/scholenopdekaart data importer.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/DUO/views.sql` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/DUO/views.sql`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/20230213 vo onderwijstype.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/20230213 vo onderwijstype.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/21.11.25-Omgeving Leiden verhuizen.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/21.11.25-Omgeving Leiden verhuizen.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/IOL_import.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/IOL_import.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/Leids aanbod uit Ghost overzetten.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/Leids aanbod uit Ghost overzetten.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/Locatiegegevens aan Organisatie.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/Locatiegegevens aan Organisatie.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/eddie-icon.png` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/eddie-icon.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/opruimen_van_eddie_tags.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/opruimen_van_eddie_tags.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/Eenmalig uitvoeren/qrcode demo.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/Eenmalig uitvoeren/qrcode demo.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/caching/caching-icm-shared-code.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/caching/caching-icm-shared-code.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/caching/caching.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/caching/caching.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/sync/federation.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/sync/federation.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/jupyterlab/notebooks/sync/synchronize.ipynb` & `ontwikkelstraat-1.19.0/jupyterlab/notebooks/sync/synchronize.ipynb`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/locust/docker-compose.yml` & `ontwikkelstraat-1.19.0/locust/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/locust/locust_static_ghost.py` & `ontwikkelstraat-1.19.0/locust/locust_static_ghost.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/locust/locustfile.py` & `ontwikkelstraat-1.19.0/locust/locustfile.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/migrate/Dockerfile` & `ontwikkelstraat-1.19.0/migrate/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,30 @@
 RUN groupadd --gid 1050 microservices && useradd --uid 1050 -g microservices microservices
 
 # onderstaande wordt telkens overschreven vanuit de docker-compose file
 # om de bewuste microservice te starten, maar wel allemaal op basis van deze image.
 ARG PIP_INDEX_URL
 ENV PIP_INDEX_URL=${PIP_INDEX_URL}
 RUN mkdir /home/microservices && chown microservices:microservices /home/microservices
-COPY migrate/requirements.txt /home/microservices
 
 RUN pip install pipx uv
 
 # uv specific (requires venv):
 ENV VIRTUAL_ENV="/opt/venv"
 RUN uv venv ${VIRTUAL_ENV}
 ENV PATH="${VIRTUAL_ENV}/bin:$PATH"
 
-RUN uv pip install -r /home/microservices/requirements.txt
 USER microservices
-# install as the microservices user, and authenticate accordingliy
+# install as the microservices user, and authenticate accordingly
 RUN pipx install b2
 ARG B2_ATTACHMENTS_KEYID
 ARG B2_ATTACHMENTS_KEY
 RUN if [ "${B2_ATTACHMENTS_KEYID}" ]; then ~/.local/bin/b2 authorize-account ${B2_ATTACHMENTS_KEYID} ${B2_ATTACHMENTS_KEY}; fi;
+
+USER root
+COPY migrate/requirements.txt /home/microservices
+RUN uv pip install -r /home/microservices/requirements.txt
+
+USER microservices
 ## expects a config file, use EDWH_MICROSERVICES_CONFIG in the environment, or use --config=filename
 CMD python3 /shared_code/edwh/core/migrate.py
```

### Comparing `ontwikkelstraat-1.18.1/migrate/requirements.in` & `ontwikkelstraat-1.19.0/migrate/requirements.in`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/migrate/requirements.txt` & `ontwikkelstraat-1.19.0/migrate/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile migrate/requirements.in --output-file migrate/requirements.txt
+#    uv pip compile migrate/requirements.in --output-file migrate/requirements.txt --upgrade
 amqp==5.2.0
     # via kombu
 anyio==4.3.0
     # via httpx
-async-timeout==4.0.3
-    # via redis
 attrs==23.2.0
 bcrypt==4.1.2
 billiard==4.2.0
     # via celery
 celery==5.3.6
 certifi==2024.2.2
     # via
@@ -22,15 +20,15 @@
     # via requests
 click==8.1.7
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
 colorlog==6.8.2
 configuraptor==1.26.2
@@ -38,46 +36,44 @@
 cryptography==42.0.5
     # via pyjwt
 dill==0.3.8
 diskcache==5.6.3
 dotmap==1.3.30
 edwh-ghost==0.1.9
 edwh-migrate==0.8.0
-exceptiongroup==1.2.0
-    # via anyio
-filelock==3.13.1
+filelock==3.13.4
 h11==0.14.0
     # via httpcore
-httpcore==1.0.4
+httpcore==1.0.5
     # via httpx
 httpx==0.27.0
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   httpx
     #   requests
     #   yarl
 invoke==2.2.0
 iso3166==2.1.1
-kombu==5.3.5
+kombu==5.3.6
     # via celery
 libsass==0.23.0
     # via pysass
 markdown2==2.4.13
 more-itertools==10.2.0
 multidict==6.0.5
     # via yarl
 plumbum==1.8.2
     # via edwh-migrate
 prompt-toolkit==3.0.43
     # via click-repl
 psycopg2-binary==2.9.9
     # via edwh-migrate
 pybars4==0.9.13
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pydal==20231114.3
     # via edwh-migrate
 pyjwt==2.8.0
     # via edwh-ghost
 pymeta3==0.5.1
     # via pybars4
@@ -108,20 +104,19 @@
 tabulate==0.9.0
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via configuraptor
 tomli-w==1.0.0
     # via configuraptor
-typeguard==4.1.5
+typeguard==4.2.1
     # via configuraptor
 typing==3.7.4.3
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
-    #   anyio
     #   configuraptor
     #   typeguard
 tzdata==2024.1
     # via celery
 ua-parser==0.18.0
     # via user-agents
 urllib3==2.2.1
```

### Comparing `ontwikkelstraat-1.18.1/migrate/data/empty.sql` & `ontwikkelstraat-1.19.0/migrate/data/empty.sql`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/playwright_test/conftest.py` & `ontwikkelstraat-1.19.0/playwright_test/conftest.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/playwright_test/test_static_ghost.py` & `ontwikkelstraat-1.19.0/playwright_test/test_static_ghost.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/Dockerfile` & `ontwikkelstraat-1.19.0/py4web/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 ENV DOCKERIZE_VERSION v0.6.1
 RUN wget https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
     && tar -C /usr/local/bin -xzvf dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
     && rm dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz
 
 # p7zip-full and aria2 are fully optional a.t.m.
 RUN groupadd --gid 1050 microservices && useradd --uid 1050 -g microservices microservices
+RUN mkdir /home/microservices
+RUN chown -R microservices:microservices /home/microservices
 
 ARG PIP_INDEX_URL
 RUN export PIP_INDEX_URL=${PIP_INDEX_URL}
 RUN pip install uv pipx
 
 # uv specific (requires venv):
 ENV VIRTUAL_ENV="/opt/venv"
@@ -34,17 +36,16 @@
 EXPOSE 7999
 
 # install all the applicatoin requirements in the global environment. it's a container, so no need to use venv
 COPY py4web/requirements.txt /p4w/requirements.txt
 RUN uv pip install --upgrade --no-cache -r /p4w/requirements.txt
 
 # run py4web and have it bind to the outside ip addresses
-#CMD ["py4web", "run", "-H", "0.0.0.0", "-p", "./password.txt", "apps", "--watch","sync", "--server","waitress","--number_workers","16"]
+# CMD ["py4web", "run", "-H", "0.0.0.0", "-p", "./password.txt", "apps", "--watch","sync", "--server","waitress","--number_workers","16"]
 # for --thunder-lock see https://uwsgi-docs.readthedocs.io/en/latest/articles/SerializingAccept.html
-#RUN pip install pydevd-pycharm~=221.6008.17
-RUN mkdir /home/microservices
-RUN chown -R microservices:microservices /home/microservices
+# RUN pip install pydevd-pycharm~=221.6008.17
+
 USER microservices
 ENV PATH=/home/microservices/.local/bin:$PATH
 CMD ["uwsgi", "--http", ":8000", "--wsgi-file", "py4web_wsgi.py", "--master", "--processes", "1", "--threads", "12", "--stats", "0.0.0.0:7999","--thunder-lock", "--touch-reload", "/p4w/reload.uwsgi"]
 # dev:
-# CMD ["py4web", "run", "-H", "0.0.0.0", "-p", "./password.txt", "apps", "--watch", "sync", "--server", "tornado"]
+# CMD ["py4web", "run", "-H", "0.0.0.0", "-p", "./password.txt", "apps", "--watch", "sync", "--server", "tornado"]
```

### Comparing `ontwikkelstraat-1.18.1/py4web/py4web_bjoern.py` & `ontwikkelstraat-1.19.0/py4web/py4web_bjoern.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/requirements.in` & `ontwikkelstraat-1.19.0/py4web/requirements.in`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/requirements.txt` & `ontwikkelstraat-1.19.0/py4web/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile py4web/requirements.in --output-file py4web/requirements.txt
+#    uv pip compile py4web/requirements.in --output-file py4web/requirements.txt --upgrade
 amqp==5.2.0
     # via kombu
 anyio==4.3.0
     # via httpx
-async-timeout==4.0.3
-    # via redis
 attrs==23.2.0
 bcrypt==4.1.2
 beautifulsoup4==4.12.3
 billiard==4.2.0
     # via celery
 bjoern==3.2.2
 celery==5.3.6
@@ -25,15 +23,15 @@
 click==8.1.7
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   py4web
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
 colorama==0.4.6
     # via py4web
@@ -47,41 +45,39 @@
     #   py4web
     #   pyjwt
 dill==0.3.8
 diskcache==5.6.3
 dotmap==1.3.30
 edwh-ghost==0.1.9
 edwh-migrate==0.8.0
-exceptiongroup==1.2.0
-    # via anyio
-filelock==3.13.1
+filelock==3.13.4
 h11==0.14.0
     # via httpcore
-httpcore==1.0.4
+httpcore==1.0.5
     # via httpx
 httpx==0.27.0
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   httpx
     #   requests
     #   yarl
 invoke==2.2.0
 iso3166==2.1.1
-kombu==5.3.5
+kombu==5.3.6
     # via celery
 libsass==0.23.0
     # via pysass
 markdown2==2.4.13
 more-itertools==10.2.0
 multidict==6.0.5
     # via yarl
 ombott==1.0.0
     # via py4web
-pillow==10.2.0
+pillow==10.3.0
     # via qrcode
 plumbum==1.8.2
     # via edwh-migrate
 pluralize==20231008.1
     # via py4web
 portalocker==2.8.2
     # via py4web
@@ -89,15 +85,15 @@
     # via click-repl
 psycopg2-binary==2.9.9
     # via edwh-migrate
 py4web==1.20220928.1
     # via py4web-debug-tools
 py4web-debug-tools==1.2.0
 pybars4==0.9.13
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pycryptodome==3.20.0
     # via py4web
 pydal==20231114.3
     # via
     #   edwh-migrate
     #   py4web
@@ -120,15 +116,15 @@
 python-slugify==8.0.4
 pytz==2024.1
 pyyaml==6.0.1
     # via configuraptor
 qrcode==7.4.2
 redis==5.0.3
     # via edwh-migrate
-renoir==1.7.0
+renoir==1.7.1
     # via py4web
 requests==2.31.0
     # via
     #   configuraptor
     #   edwh-ghost
     #   py4web
 rocket3==20231022.2
@@ -149,19 +145,18 @@
     # via py4web
 tomli==2.0.1
     # via configuraptor
 tomli-w==1.0.0
     # via configuraptor
 tornado==6.4
     # via py4web
-typeguard==4.1.5
+typeguard==4.2.1
     # via configuraptor
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
-    #   anyio
     #   configuraptor
     #   qrcode
     #   typeguard
 tzdata==2024.1
     # via celery
 ua-parser==0.18.0
     # via user-agents
```

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/c/__init__.py` & `ontwikkelstraat-1.19.0/py4web/apps/c/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/__init__.py` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/demo.py` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/demo.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/fixtures.py` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/fixtures.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/handlebars.py` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/handlebars.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/opengraph.py` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/opengraph.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/settings.py` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/settings.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/src/sass/main.scss` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/src/sass/main.scss`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/fonts.css` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/fonts.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/mystyles.css` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/banner.webp` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/banner.webp`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/boy.png` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/boy.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-by.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-by.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-general.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-general.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-nc-eu.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-nc-eu.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-nd.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-nd.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-remix.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-remix.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-sa.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-sa.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-share.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-share.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/cc-zero.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/cc-zero.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/de-pionier.png` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/de-pionier.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/elders.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/elders.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/email.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/email.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/grootte.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/grootte.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/hier.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/hier.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/hs-leiden.png` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/hs-leiden.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/icon.png` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/info.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/info.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/kennis.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/kennis.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/logo.png` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/onderwijsniveau.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/onderwijsniveau.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/onderwijstype.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/onderwijstype.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/pd.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/pd.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/pencil-solid.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/pencil-solid.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/profiel.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/profiel.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/seal.png` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/seal.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/images/users-solid.svg` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/images/users-solid.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/_hyperscript_w9y-0.9.3.min.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/_hyperscript_w9y-0.9.3.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/_hyperscript_w9y-0.9.5-dev.min.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/_hyperscript_w9y-0.9.5-dev.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/_hyperscript_w9y-dev.min.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/_hyperscript_w9y-dev.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/_hyperscript_w9y.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/_hyperscript_w9y.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/behaviors._hs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/behaviors._hs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/browser-report.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/browser-report.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/bulma.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/bulma.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/commands._hs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/commands._hs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/htmx.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/htmx.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/htmx_extend.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/htmx_extend.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/javascript_dependencies.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/javascript_dependencies.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/static/js/leaflet-providers.js` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/static/js/leaflet-providers.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/activiteiten.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/activiteiten.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/demo.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/demo.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/demo_template.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/demo_template.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/extern.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/extern.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/hotspots.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/hotspots.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/index.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/index.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/item.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/item.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/item.html` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/item.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/leiden.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/leiden.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/ratings.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/ratings.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/school.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/school.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/school.html` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/school.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/template-item.html` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/template-item.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/template.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/template.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/template.html` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/template.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/template_minimal.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/template_minimal.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/user.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/user.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/cmsx/templates/user.html` & `ontwikkelstraat-1.19.0/py4web/apps/cmsx/templates/user.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/__init__.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/backend_support.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/backend_support.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/common.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/common.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/controllers.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/controllers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/fixtures.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/fixtures.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/handlebars.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/handlebars.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/helpers.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/helpers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/hotspots.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/hotspots.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/models.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/models.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/settings.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/settings.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/tasks.py` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/tasks.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/databases/plaatsen.json` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/databases/plaatsen.json`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/databases/slugified_plaatsen.json` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/databases/slugified_plaatsen.json`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/css/bundled-latest.css` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/css/bundled-latest.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/css/no.css` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/css/no.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/banner.webp` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/banner.webp`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/boy.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/boy.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-by.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-by.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-general.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-general.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-nc-eu.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-nc-eu.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-nd.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-nd.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-remix.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-remix.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-sa.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-sa.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-share.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-share.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/cc-zero.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/cc-zero.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/de-pionier.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/de-pionier.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/elders.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/elders.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/email.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/email.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/grootte.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/grootte.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/hier.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/hier.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/hs-leiden.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/hs-leiden.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/icon.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/info.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/info.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/kennis.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/kennis.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/onderwijsniveau.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/onderwijsniveau.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/onderwijstype.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/onderwijstype.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/pd.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/pd.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/pencil-solid.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/pencil-solid.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/profiel.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/profiel.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/seal.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/seal.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/users-solid.svg` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/users-solid.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/a.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/a.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/b.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/b.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/c.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/c.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/d.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/d.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/e.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/e.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/f.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/f.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/g.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/g.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/h.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/h.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/i.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/i.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/j.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/j.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/k.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/k.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/l.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/l.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/m.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/m.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/n.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/n.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/o.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/o.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/p.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/p.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/q.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/q.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/r.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/r.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/s.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/s.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/t.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/t.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/u.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/u.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/v.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/v.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/w.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/w.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/x.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/x.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/y.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/y.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/images/thumbnails/z.png` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/images/thumbnails/z.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/js/bundled-latest.js` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/js/bundled-latest.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/static/js/utils.js` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/static/js/utils.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/active_filters.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/active_filters.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/external_tiles.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/external_tiles.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/hotspots.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/hotspots.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/hotspots.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/hotspots.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/item.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/item.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/item.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/item.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/layout.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/layout.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/menu.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/menu.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/menu.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/menu.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/modals.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/modals.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/modals.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/modals.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/notification.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/notification.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/notification.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/notification.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/rating_form.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/rating_form.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/rating_results.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/rating_results.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/school.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/school.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/school.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/school.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/tiles.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/tiles.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/tiles.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/tiles.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/user.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/user.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/user.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/user.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/email_validate.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/email_validate.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/email_validate.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/email_validate.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/login.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/login.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/login.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/no_cookies.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/no_cookies.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/recover.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/recover.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/recover.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/recover.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/register1.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/register1.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/register1.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/register1.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/register2.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/register2.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/auth/register2.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/auth/register2.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filterbuttons.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filterbuttons.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filterbuttons.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filterbuttons.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filtermenu-modal.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filtermenu-modal.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filtermenu-modal.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filtermenu-modal.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filtermenu.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filtermenu.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/fragmentx/templates/partials/filtermenu.html` & `ontwikkelstraat-1.19.0/py4web/apps/fragmentx/templates/partials/filtermenu.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/controllers.py` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/controllers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/handlebars.py` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/handlebars.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/helpers.py` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/helpers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/klassen_enquete.py` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/klassen_enquete.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/static/css/no.css` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/static/css/no.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/static/js/utils.js` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/static/js/utils.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/klassen_index.html` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/klassen_index.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/layout.html` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/layout.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/enquete_uitslag.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/enquete_uitslag.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/stapel.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/stapel.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/thema_uitleg.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/thema_uitleg.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/thema_uitleg_schoolleider.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/thema_uitleg_schoolleider.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/gelijkekansen/templates/kansen/vraag.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/gelijkekansen/templates/kansen/vraag.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/__init__.py` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/demo.py` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/demo.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/fixtures.py` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/fixtures.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/handlebars.py` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/handlebars.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/opengraph.py` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/opengraph.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/settings.py` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/settings.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/src/sass/main.scss` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/src/sass/main.scss`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/fonts.css` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/fonts.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/mystyles.css` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/banner.webp` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/banner.webp`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/boy.png` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/boy.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/cc-by.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/cc-by.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/cc-general.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/cc-general.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/cc-sa.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/cc-sa.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/de-pionier.png` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/de-pionier.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/elders.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/elders.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/email.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/email.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/grootte.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/grootte.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/hier.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/hier.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/hs-leiden.png` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/hs-leiden.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/info.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/info.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/kennis.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/kennis.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/logo.png` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/onderwijsniveau.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/onderwijsniveau.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/onderwijstype.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/onderwijstype.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/images/profiel.svg` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/images/profiel.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-0.9.3.min.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-0.9.3.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-0.9.5-dev.min.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-0.9.5-dev.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-dev.min.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/_hyperscript_w9y-dev.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/_hyperscript_w9y.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/_hyperscript_w9y.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/behaviors._hs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/behaviors._hs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/browser-report.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/browser-report.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/bulma.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/bulma.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/commands._hs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/commands._hs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/htmx.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/htmx.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/htmx_extend.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/htmx_extend.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/javascript_dependencies.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/javascript_dependencies.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/static/js/leaflet-providers.js` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/static/js/leaflet-providers.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/activiteiten.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/activiteiten.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/demo.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/demo.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/demo_template.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/demo_template.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/extern.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/extern.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/hotspots.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/hotspots.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/index.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/index.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/item.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/item.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/item.html` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/item.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/leiden.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/leiden.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/ratings.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/ratings.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/school.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/school.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/school.html` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/school.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/template-item.html` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/template-item.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/template.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/template.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/template.html` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/template.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/template_minimal.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/template_minimal.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/user.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/user.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/iolrapportage/templates/user.html` & `ontwikkelstraat-1.19.0/py4web/apps/iolrapportage/templates/user.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/jwt_demo/__init__.py` & `ontwikkelstraat-1.19.0/py4web/apps/jwt_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/common.py` & `ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/common.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/controllers.py` & `ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/controllers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/ghost.py` & `ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/ghost.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/handlebars.py` & `ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/handlebars.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/models.py` & `ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/models.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/settings.py` & `ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/settings.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/leiden-ghost-search/tasks.py` & `ontwikkelstraat-1.19.0/py4web/apps/leiden-ghost-search/tasks.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/__init__.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/backend_support.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/backend_support.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/common.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/common.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/common_lts.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/common_lts.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/controllers.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/controllers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/fixtures.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/fixtures.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/fixtures_lts.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/fixtures_lts.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/graphql_support.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/graphql_support.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/handlebars.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/handlebars.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/helpers.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/helpers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/hotspots.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/hotspots.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/lts_controllers.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/lts_controllers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/markdown_template.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/markdown_template.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/models.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/models.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/models_lts.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/models_lts.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/settings.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/settings.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/tasks.py` & `ontwikkelstraat-1.19.0/py4web/apps/lts/tasks.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/databases/lts_assets.sql` & `ontwikkelstraat-1.19.0/py4web/apps/lts/databases/lts_assets.sql`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/databases/plaatsen.json` & `ontwikkelstraat-1.19.0/py4web/apps/lts/databases/plaatsen.json`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/databases/slugified_plaatsen.json` & `ontwikkelstraat-1.19.0/py4web/apps/lts/databases/slugified_plaatsen.json`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/css/bundled-1.0.0.css` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/css/bundled-1.0.0.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/css/bundled.css` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/css/bundled.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/css/no.css` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/css/no.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/banner.webp` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/banner.webp`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/boy.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/boy.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-by.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-by.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-general.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-general.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-nc-eu.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-nc-eu.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-nd.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-nd.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-remix.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-remix.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-sa.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-sa.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-share.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-share.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/cc-zero.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/cc-zero.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/de-pionier.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/de-pionier.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/elders.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/elders.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/email.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/email.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/grootte.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/grootte.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/hier.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/hier.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/hs-leiden.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/hs-leiden.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/icon.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/info.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/info.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/kennis.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/kennis.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/onderwijsniveau.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/onderwijsniveau.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/onderwijstype.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/onderwijstype.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/pd.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/pd.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/pencil-solid.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/pencil-solid.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/profiel.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/profiel.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/seal.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/seal.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/users-solid.svg` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/users-solid.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/a.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/a.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/b.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/b.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/c.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/c.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/d.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/d.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/e.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/e.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/f.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/f.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/g.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/g.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/h.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/h.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/i.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/i.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/j.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/j.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/k.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/k.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/l.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/l.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/m.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/m.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/n.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/n.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/o.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/o.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/p.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/p.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/q.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/q.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/r.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/r.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/s.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/s.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/t.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/t.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/u.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/u.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/v.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/v.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/w.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/w.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/x.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/x.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/y.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/y.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/images/thumbnails/z.png` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/images/thumbnails/z.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/js/bundled-1.0.0.js` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/js/bundled-1.0.0.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/js/bundled.js` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/js/bundled.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/static/js/utils.js` & `ontwikkelstraat-1.19.0/py4web/apps/lts/static/js/utils.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/active_filters.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/active_filters.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/documentatie.md` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/documentatie.md`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/email_registration_form.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/email_registration_form.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/email_registration_form.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/email_registration_form.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/enquete_uitslag.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/enquete_uitslag.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/external_tiles.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/external_tiles.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/external_tiles.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/external_tiles.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/hotspots.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/hotspots.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/hotspots.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/hotspots.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/item.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/item.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/item.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/item.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/klassen_index.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/klassen_index.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/layout.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/layout.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/menu.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/menu.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/menu.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/menu.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/modals.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/modals.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/modals.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/modals.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/notification.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/notification.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/notification.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/notification.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/rating_form.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/rating_form.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/rating_results.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/rating_results.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/school.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/school.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/school.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/school.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/stapel.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/stapel.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/thema_uitleg.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/thema_uitleg.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/tiles.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/tiles.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/tiles.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/tiles.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/user.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/user.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/user.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/user.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/vraag.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/vraag.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/email_validate.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/email_validate.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/email_validate.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/email_validate.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/login.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/login.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/login.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/recover.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/recover.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/recover.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/recover.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/register1.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/register1.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/register1.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/register1.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/register2.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/register2.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/auth/register2.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/auth/register2.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/layouts/generic.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/layouts/generic.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/layouts/markdown.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/layouts/markdown.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_2.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_2.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_3.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_3.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_layout.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_layout.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/builder_tags.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/builder_tags.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/demo.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/demo.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/manage_grid.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/manage_grid.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/lts/manage_groups.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/lts/manage_groups.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filterbuttons.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filterbuttons.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filterbuttons.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filterbuttons.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filtermenu-modal.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filtermenu-modal.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filtermenu-modal.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filtermenu-modal.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filtermenu.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filtermenu.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/lts/templates/partials/filtermenu.html` & `ontwikkelstraat-1.19.0/py4web/apps/lts/templates/partials/filtermenu.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/__init__.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/backend_support.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/backend_support.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/common.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/common.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/controllers.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/controllers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/fixtures.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/fixtures.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/handlebars.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/handlebars.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/helpers.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/helpers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/settings.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/settings.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/tasks.py` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/tasks.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/LEF logo.svg` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/LEF logo.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/Onderwijsindeleidseregio logo.svg` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/Onderwijsindeleidseregio logo.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/icon.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/a.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/a.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/b.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/b.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/c.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/c.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/d.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/d.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/e.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/e.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/f.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/f.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/g.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/g.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/h.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/h.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/i.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/i.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/j.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/j.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/k.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/k.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/l.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/l.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/m.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/m.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/n.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/n.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/o.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/o.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/p.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/p.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/q.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/q.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/r.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/r.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/s.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/s.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/t.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/t.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/u.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/u.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/v.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/v.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/w.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/w.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/x.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/x.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/y.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/y.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/static/images/thumbnails/z.png` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/static/images/thumbnails/z.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/narrowcasting/templates/narrowcasting.html` & `ontwikkelstraat-1.19.0/py4web/apps/narrowcasting/templates/narrowcasting.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/restart/__init__.py` & `ontwikkelstraat-1.19.0/py4web/apps/restart/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/restart/static/favicon.ico` & `ontwikkelstraat-1.19.0/py4web/apps/restart/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/common.py` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/common.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/controllers.py` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/controllers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/handlebars.py` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/handlebars.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/models.py` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/models.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/settings.py` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/settings.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/tasks.py` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/tasks.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/databases/dna.csv` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/databases/dna.csv`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/card.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/card.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/ghost.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/ghost.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/index.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/index.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/uitslag.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/uitslag.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/py4web/apps/slimfit-plaatsbepaling/templates/vraag.hbs` & `ontwikkelstraat-1.19.0/py4web/apps/slimfit-plaatsbepaling/templates/vraag.hbs`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/data_model.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,15 @@
             requires=IS_EMPTY_OR(IS_IN_DB(database, "tag.gid", "%(name)s")),
             comment="De tag moet al bestaan, deze kun je aanmaken via het Tags menu en hier koppelen. "
             "Let op: de tag moet de parent 'Organisations' hebben!",
         ),
         Field(
             "lonlat",
             "point",
-            comment="`(4.4678539,52.1414083)` bijvoorbeeld. Point type, longitude-lattitude",
+            comment="`(4.4678539,52.1414083)` bijvoorbeeld. Point type, longitude-latitude (net andersom dan google)",
             label="Coordinaten",
         ),
         Field(
             "scholen_op_de_kaart_url",
             "string",
             length=512,
             requires=IS_EMPTY_OR(IS_HTTP_URL()),
@@ -629,14 +629,18 @@
         ),
         Field(
             "last_saved_by", "string", default=None, writable=False
         ),  # autopopulation set in the web2py model
         # Field.Virtual("needle", lambda row: f'{row.name} {row.city}'),
     )
 
+    database.organisation.latlon = Field.Virtual(
+        lambda row: tuple(row.organisation.lonlat.strip("()").split(",")[::-1])
+    )
+
     database.define_table(
         "organisation_effdted_now",
         organisation,
         migrate=False,
         rname="organisation_effdted_now",
     )
```

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/migrations.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/migrations.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/tags.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/tags.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/asink.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/asink.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/celerysink.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/celerysink.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/diskcachesink.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/diskcachesink.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/signalemitter.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/signalemitter.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/sink.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/sink.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/applog/tasks.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/applog/tasks.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/engine.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/engine.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/ntfy_sh.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/ntfy_sh.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/opengraph.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/opengraph.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/support.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/support.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/backend/tasks.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/backend/tasks.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/jwt_tools/jwt_py4web.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/jwt_tools/jwt_py4web.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/jwt_tools/jwt_web2py.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/jwt_tools/jwt_web2py.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/jwt_tools/shared.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/jwt_tools/shared.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/pgcache/__init__.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/pgcache/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/pgcache/clean.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/pgcache/clean.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/sync/__init__.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/shared_code/edwh/core/web2py_tools/__init__.py` & `ontwikkelstraat-1.19.0/shared_code/edwh/core/web2py_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/Dockerfile` & `ontwikkelstraat-1.19.0/web2py/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 RUN pip install uv pipx
 
 # uv specific (requires venv):
 ENV VIRTUAL_ENV="/opt/venv"
 RUN uv venv ${VIRTUAL_ENV}
 ENV PATH="${VIRTUAL_ENV}/bin:$PATH"
 
+# installeert web2py naar /src/web2py (normale pip want 'uv' crasht op web2py's rare versienummers)
+RUN pip install --no-cache -e git+https://github.com/web2py/web2py@v2.22.5#egg=web2py
+
 # keep app requirements in the project folder on the devel machine. p4w-test here in the screenshot below.
 COPY web2py/requirements.txt /w2p/requirements.txt
 
 # install all the applicatoin requirements in the global environment. it's a container, so no need to use venv
 RUN uv pip install --no-cache -r /w2p/requirements.txt
-# installeert web2py naar /src/web2py (normale pip want 'uv' crasht op web2py's rare versienummers)
-RUN pip install --no-cache -e git+https://github.com/web2py/web2py@v2.22.5#egg=web2py
 
 # chdir to the directory where password and apps folder is, this is the base
 # directory from which to start py4web.
 WORKDIR  /src/web2py
 RUN chown microservices:microservices -R /src/web2py
 # expose py4web on it's default port
 EXPOSE 8000
```

### Comparing `ontwikkelstraat-1.18.1/web2py/requirements.in` & `ontwikkelstraat-1.19.0/web2py/requirements.in`

 * *Files 2% similar despite different names*

```diff
@@ -42,11 +42,13 @@
 pyjwt[crypto]
 attrs
 edwh-migrate>=0.4.3
 yarl
 humanize
 edwh-web2py-effdted-prio-grid>=0.1.2
 invoke
+geopy
+
 #########################################
 # PINNED VERSIONS FOR SECURITY REASONS: #
 #########################################
 urllib3>=1.26.18,<2 # v2 maakt requests in web2py stuk, dus gebruik de laatste patch van v1!
```

### Comparing `ontwikkelstraat-1.18.1/web2py/requirements.txt` & `ontwikkelstraat-1.19.0/web2py/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile web2py/requirements.in --output-file web2py/requirements.txt
 amqp==5.2.0
     # via kombu
 anyio==4.3.0
     # via httpx
-async-timeout==4.0.3
-    # via redis
 attrs==23.2.0
 bcrypt==4.1.2
 beautifulsoup4==4.12.3
     # via html2markdown
 billiard==4.2.0
     # via celery
 celery==5.3.6
@@ -24,81 +22,80 @@
     # via requests
 click==8.1.7
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
 colorlog==6.8.2
 configuraptor==1.26.2
     # via edwh-migrate
 cryptography==42.0.5
     # via pyjwt
 dill==0.3.8
 diskcache==5.6.3
 edwh-migrate==0.8.0
 edwh-web2py-effdted-prio-grid==0.1.2
-exceptiongroup==1.2.0
-    # via
-    #   anyio
-    #   pytest
-execnet==2.0.2
+execnet==2.1.1
     # via pytest-xdist
-filelock==3.13.1
+filelock==3.13.4
+geographiclib==2.0
+    # via geopy
+geopy==2.4.1
 greenlet==3.0.3
     # via playwright
 h11==0.14.0
     # via httpcore
 html2markdown==0.1.7
-httpcore==1.0.4
+httpcore==1.0.5
     # via httpx
 httpx==0.27.0
 humanize==4.9.0
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   httpx
     #   requests
     #   yarl
 iniconfig==2.0.0
     # via pytest
 invoke==2.2.0
 iso3166==2.1.1
-kombu==5.3.5
+kombu==5.3.6
     # via celery
 libsass==0.23.0
     # via pysass
 markdown2==2.4.13
 more-itertools==10.2.0
 multidict==6.0.5
     # via yarl
 packaging==24.0
     # via pytest
-playwright==1.42.0
+playwright==1.43.0
     # via pytest-playwright
 pluggy==1.4.0
     # via pytest
 plumbum==1.8.2
     # via edwh-migrate
 prompt-toolkit==3.0.43
     # via click-repl
 psycopg2-binary==2.9.9
     # via edwh-migrate
 pybars4==0.9.13
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pydal==20231114.3
     # via edwh-migrate
-pyee==11.0.1
+pyee==11.1.0
     # via playwright
 pyjwt==2.8.0
 pymeta3==0.5.1
     # via pybars4
 pysass==0.1.0
 pytest==8.1.1
     # via
@@ -133,24 +130,21 @@
     #   httpx
 soupsieve==2.5
     # via beautifulsoup4
 tabulate==0.9.0
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
-    # via
-    #   configuraptor
-    #   pytest
+    # via configuraptor
 tomli-w==1.0.0
     # via configuraptor
-typeguard==4.1.5
+typeguard==4.2.1
     # via configuraptor
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
-    #   anyio
     #   configuraptor
     #   pyee
     #   typeguard
 tzdata==2024.1
     # via celery
 ua-parser==0.18.0
     # via user-agents
```

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/routes.example.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/routes.example.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/controllers/appadmin.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/controllers/appadmin.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/controllers/default.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/controllers/default.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/ar.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/ar.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/ca.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/ca.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/cs.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/cs.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/de.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/de.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/en.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/en.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/es.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/es.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/fr-ca.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/fr-ca.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/fr.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/fr.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/hi.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/hi.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/hu.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/hu.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/id.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/id.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/it.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/it.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/my-mm.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/my-mm.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/my.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/my.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/nl.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/nl.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/pl.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/pl.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/plural-cs.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/plural-cs.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/plural-ru.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/plural-ru.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/plural-uk.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/plural-uk.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/pt-br.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/pt-br.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/pt.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/pt.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/ro.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/ro.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/ru.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/ru.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/sk.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/sk.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/tr.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/tr.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/uk.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/uk.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/zh-cn.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/zh-cn.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/zh-tw.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/zh-tw.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/languages/zh.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/languages/zh.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/models/db.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/models/db.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/models/menu.py` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/models/menu.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/private/appconfig.ini` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/private/appconfig.ini`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/bootstrap.min.css` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/bootstrap.min.css.map` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/calendar.css` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/calendar.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/web2py-bootstrap4.css` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/web2py-bootstrap4.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/css/web2py.css` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/css/web2py.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/images/facebook.png` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/images/facebook.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/images/gplus-32.png` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/images/gplus-32.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/images/twitter.png` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/images/twitter.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/analytics.min.js` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/analytics.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/bootstrap.bundle.min.js` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/bootstrap.bundle.min.js.map` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/calendar.js` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/calendar.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/jquery.js` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/jquery.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/modernizr-2.8.3.min.js` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/modernizr-2.8.3.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/web2py-bootstrap4.js` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/web2py-bootstrap4.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/static/js/web2py.js` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/static/js/web2py.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/appadmin.html` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/appadmin.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.csv` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.csv`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.ics` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.ics`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.jsonp` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.jsonp`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.load` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.load`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/generic.map` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/generic.map`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/layout.html` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/layout.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/web2py_ajax.html` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/web2py_ajax.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/ioldb/views/default/user.html` & `ontwikkelstraat-1.19.0/web2py/apps/ioldb/views/default/user.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/errors.tgz` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/errors.tgz`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/progress.log` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/progress.log`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/routes.example.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/routes.example.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/api.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/api.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/appadmin.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/appadmin.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/applog.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/applog.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/default.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -1173,15 +1173,15 @@
     ]
     links = [
         dict(
             header="Bekijk",
             body=lambda row: A(
                 XML("Bekijk op website"),
                 _href=f"https://{os.getenv('APPLICATION_NAME')}.{os.getenv('HOSTINGDOMAIN')}/item/"
-                + row.gid,
+                      + row.gid,
                 _target="_blank",
                 _class="btn btn-primary",
             ),
         ),
         dict(
             header="Bewerk",
             body=lambda row: A(
@@ -1368,15 +1368,15 @@
         # geeft de form een button 'Reset wachtwoord' die naar de functie form_process gaat
         # met als argument de request.args die hiervoor meegegeven was.
         buttons=[
             BUTTON(
                 "Reset wachtwoord",
                 _type="button",
                 _onClick="parent.location='%s'"
-                % URL(f="password_reset_confirmed", args=request.args[0]),
+                         % URL(f="password_reset_confirmed", args=request.args[0]),
             )
         ],
     )
     return dict(form=form)
 
 
 @auth.requires_membership("education_warehouse")
@@ -1678,32 +1678,32 @@
         )
     }
 
     auto_tag.tagged_in_db.writable = False
     auto_tag.search_results.writable = False
 
     def item_gid_as_link(gid, record, with_untag_button=False):
-        full_name = item_gid_map[gid]
+        full_name = item_gid_map.get(gid, "?")
         short_name = XML(
             textwrap.shorten(full_name, width=30, placeholder="&mldr;")  # …
         )
 
         untag_button = (
             A(
                 XML("&#10060;"),  # ❌
                 _href=URL(
                     f="untag",
                     args=[gid, record.tag_gid],
                 ),
                 _style="font-size:0.8rem;",
                 _title="Verwijder deze tag.",
                 _onclick="return confirm('"
-                "Weet je zeker dat je deze tag wilt ontkoppelen? "
-                "Het zou kunnen dat het automatisch weer wordt toegevoegd indien de zoektag matcht."
-                "')",
+                         "Weet je zeker dat je deze tag wilt ontkoppelen? "
+                         "Het zou kunnen dat het automatisch weer wordt toegevoegd indien de zoektag matcht."
+                         "')",
             )
             if with_untag_button
             else ""
         )
 
         return SPAN(
             A(short_name, _title=full_name, _href=URL("quick_edit", args=[gid])),
@@ -1734,17 +1734,24 @@
             item_gids_as_links,
             with_untag_button=False,
         )
     else:
         auto_tag.tagged_in_db.readable = False
         auto_tag.search_results.readable = False
 
-    auto_tag.tag_gid.represent = lambda gid, record: A(
-        database.tag(gid=gid).name, _href=URL("edit_tag", args=[gid]), _target="_blank"
-    )
+    def represent_auto_tag(gid: str, _record) -> A:
+        row = database.tag(gid=gid)
+
+        return A(
+            row.name if row else "(verwijderde tag)",
+            _href=URL(c="workbench", f='tag', args=[gid]),
+            _target="_blank"
+        )
+
+    auto_tag.tag_gid.represent = represent_auto_tag
     grid = SQLFORM.grid(
         auto_tag,
         searchable=True,
         advanced_search=False,
         paginate=None,
         maxtextlength=20000,
         editable=True,
```

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/dv_appadmin.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/dv_appadmin.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/jwt_auth.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/organisations.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/organisations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
+import re
 import typing
 
 import edwh.core.web2py_tools
 from edwh.core.backend.engine import OrganisationPriority, update_effectivedated
 
 # from edwh.core.web2py_tools import effective_dated_grid, hide
 from edwh_web2py_effdted_prio_grid import effective_dated_grid, hide
 from gluon.tools import prettydate
 
 if typing.TYPE_CHECKING:
-    from gluon import URL, auth, redirect, request, session
+    from gluon import URL, auth, redirect, request, session, response
     from gluon.html import PRE, SPAN, TT, XML, A
     from gluon.sqlhtml import SQLFORM
     from pydal import Field
     from pydal.validators import IS_MATCH
 
     from ..models.db import (
         database,
@@ -53,14 +54,73 @@
         onvalidation=onvalidation,
     )
     return dict(form=grid)
 
 
 ORG_GID = "e5b80b90-1851-42d9-aebc-87327e87ed09"
 
+KomootData = typing.TypedDict("KomootData", {
+    "lonlat": str,
+    "number": str,
+    "street": str,
+    "postalcode": str,
+    "city": str,
+})
+
+
+def load_geo(street: str,
+             number: str,
+             postalcode: str,
+             city: str, country="Netherlands"
+             ) -> KomootData:
+    import httpx
+    result: KomootData = {}
+
+    resp = httpx.get(
+        f"https://photon.komoot.io/api/?q={street}+{number}+{postalcode}+{city}+'{country}'",
+        headers={
+            "User-Agent": "EducationWarehouse workbench (httpx python), thanks for saving us time!"
+        },
+        timeout=10,
+    )
+
+    print(resp.json())
+    if resp.is_success:
+        js = resp.json()
+        try:
+            if not js["features"]:
+                raise KeyError("geen succes")
+
+            # save in swapped version for database
+            result['lonlat'] = "({0},{1})".format(
+                *js["features"][0]["geometry"]["coordinates"]
+            )
+            print("lonlat set:", result['lonlat'])
+        except KeyError as e:
+            print(e)
+            response.flash = "Geocoordinaten konden niet geladen worden voor het gegeven adres."
+        try:
+            if js["features"]:
+                features = js["features"][0]
+                properties = features["properties"]
+
+                result["street"] = properties["street"]
+                result["number"] = properties["housenumber"]
+                result["postalcode"] = properties["postcode"]
+                result["city"] = properties["city"]
+        except KeyError as e:
+            print(e)
+    else:
+        print(resp.content)
+        response.flash = (
+            "Geocoordinaten konden niet geladen worden voor het gegeven adres."
+        )
+
+    return result
+
 
 @auth.requires(is_eddie or is_minion)
 def index():
     warning = last_opened_warning("org")
 
     mdash = XML("&mdash;")
     organisation = database.organisation
@@ -148,16 +208,14 @@
         hide(organisation.vestigingscode)
         hide(organisation.platform)
         hide(organisation.correspondence_city)
         hide(organisation.correspondence_street)
         hide(organisation.correspondence_number)
         hide(organisation.correspondence_postalcode)
         hide(organisation.correspondence_country)
-        hide(organisation.tag_gid)
-        hide(organisation.lonlat)
         hide(organisation.country_code)
         hide(organisation.scholen_op_de_kaart_url)
         hide(organisation.sector)
         hide(organisation.education_level)
         hide(organisation.education_type)
         hide(organisation.denomination)
         hide(organisation.so_cluster)
@@ -201,14 +259,38 @@
         request,
         database.tag.name,
         database.tag.gid,
         query=database.tag.parents.contains(ORG_GID),
     )
 
     def onvalidation(form):
+        if (
+            (form.vars.street and form.vars.number and form.vars.city)
+            or (form.vars.number and form.vars.postalcode)
+        ) and not form.vars.lonlat:
+            geo_data = load_geo(form.vars.street, form.vars.number, form.vars.postalcode, form.vars.city)
+            form.vars.update(geo_data)
+        if form.vars.lonlat:
+            import geopy.distance
+            import geopy.point
+
+            try:
+                lon, lat = form.vars.lonlat.strip().strip("()").split(",")
+                lon, lat = float(lon), float(lat)
+                point = geopy.point.Point(lat, lon)
+                if point.latitude < point.longitude:
+                    # reverse lon lat
+                    # we save it as longitude latitude for geospatial functions,
+                    # but the world uses it latitude, longitude
+                    point = geopy.point.Point(point.longitude, point.latitude)
+                form.vars.lonlat = f"({point.longitude},{point.latitude})"
+            except Exception as e:
+                print(e)
+                form.errors.lonlat = str(e) + "," + str(form.vars.lonat)
+
         if tag_gid := form.vars.tag_gid:
             if isinstance(tag_gid, list) and len(tag_gid) > 1:
                 form.errors.tag_gid = "Kies maximaal één tag."
 
     def upper(value: typing.Optional[str]) -> str:
         return value.upper() if value else ""
```

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/plugin_comments.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/plugin_comments.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/scratch.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/scratch.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/webtest_support.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/webtest_support.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/controllers/workbench.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/controllers/workbench.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,16 +586,25 @@
     stickers = database().select(database.sticker.tag_gid)
     TSticker.save_reordered(database, "children", [row.tag_gid for row in stickers])
     redirect(URL(f="tag", vars={"gid": TSticker.gid}))
 
 
 @auth.requires_membership("education_warehouse")
 def tag():
-    tag_gid = request.vars.gid
+    if request.vars.gid:
+        tag_gid = request.vars.gid
+    elif request.args:
+        tag_gid = request.args[0]
+    else:
+        tag_gid = None
+
     tag = database.tag(gid=tag_gid)
+    if tag is None:
+        raise HTTP(404, f"Tag met gid {tag_gid} niet gevonden.")
+
     database.tag.id.readable = False
     database.tag.platform.readable = False
     database.tag.platform.writable = False
     database.tag.gid.writable = False
     database.tag.gid.readable = True
     database.tag.gid.represent = lambda gid, row: PRE(gid)
     database.tag.slug.writable = False
@@ -805,15 +814,14 @@
 
     md = [
         f"# {item.title}",
         f"Bij {item.contact_id.org} in {item.contact_id.location} wordt sinds {answer_per_question.get('Sinds wanneer')} "
         f"gewerkt met {answer_per_question.get('Kern van de praktijk')} om {answer_per_question.get('Aanleiding')}. ",
     ]
     for row in rows:
-
         def nice_paragraph(note):
             return textwrap.indent(textwrap.dedent(note or ""), "> ")
 
         md.append(f"## {row.question.question}")
         md.append(f"{nice_paragraph(row.item_question.note)}")
         md.append("")
         md.append("")
@@ -949,15 +957,14 @@
     exposes services. for example:
     http://..../[app]/default/call/jsonrpc
     decorate with @services.jsonrpc the functions to expose
     supports xml, json, xmlrpc, jsonrpc, amfrpc, rss, csv
     """
     return service()
 
-
 # def demo():
 #     # return response.json(asdict(backend.pratices(search=request.vars.q)))
 #     return response.json(
 #         asdict(
 #             backend.pratices(search=request.vars.q),
 #             value_serializer=serialize_backend_types,
 #             filter=filter_backend_types,
```

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_dod_rule.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_dod_rule.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_question.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_item_question.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_plugin_comments_comment.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_plugin_comments_comment.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_source_file.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/ad7992351889d8934d1e19ade550c80b_source_file.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_cas.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_cas.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_event.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_event.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_permission.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_permission.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_run.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_run.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_task.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_task.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_task_deps.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_task_deps.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_worker.table` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/c8b669d15150d7109e5f7ab36744a5b7_scheduler_worker.table`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/sql.log` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/sql.log`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/storage.sqlite` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/storage.sqlite`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/databases/workbench.sqlite` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/databases/workbench.sqlite`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/functional_test/test.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/functional_test/test.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/functional_test/tools.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/functional_test/tools.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/ca.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/ca.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/cs.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/cs.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/de.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/de.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/en.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/en.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/es.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/es.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/fr-ca.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/fr-ca.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/fr.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/fr.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/hi.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/hi.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/hu.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/hu.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/id.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/id.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/it.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/it.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/my-mm.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/my-mm.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/my.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/my.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/nl.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/nl.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/pl.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/pl.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/plural-cs.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/plural-cs.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/plural-ru.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/plural-ru.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/plural-uk.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/plural-uk.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/pt-br.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/pt-br.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/pt.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/pt.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/ro.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/ro.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/ru.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/ru.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/sk.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/sk.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/tr.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/tr.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/uk.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/uk.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/zh-cn.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/zh-cn.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/zh-tw.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/zh-tw.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/languages/zh.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/languages/zh.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/aaa_500_checkbox_widget.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/aaa_500_checkbox_widget.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/article_importers.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/article_importers.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/db.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/db.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/db_workbench.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/db_workbench.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/db_z_backend.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/db_z_backend.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/menu.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/menu.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/plugin_comments.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/plugin_comments.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/scheduler.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/models/tags.py` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/models/tags.py`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/bootstrap.min.css` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/calendar.css` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/calendar.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/edit.css` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/edit.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/master.css` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/master.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/web2py-bootstrap3.css` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/web2py-bootstrap3.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/css/web2py.css` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/css/web2py.css`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/ProximaNovaLt.otf` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/ProximaNovaLt.otf`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.eot` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.svg` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.ttf` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.woff` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.woff2` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/background.jpg` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/background.jpg`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/banner.ef18bff1.png` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/banner.ef18bff1.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/facebook.png` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/facebook.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/gplus-32.png` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/gplus-32.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/images/twitter.png` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/images/twitter.png`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/analytics.min.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/analytics.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/bootstrap.min.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/calendar.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/calendar.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/edit.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/edit.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/jquery.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/jquery.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/modernizr-2.8.3.min.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/modernizr-2.8.3.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/respond-1.4.2.min.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/respond-1.4.2.min.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/share.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/share.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/web2py-bootstrap3.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/web2py-bootstrap3.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/static/js/web2py.js` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/static/js/web2py.js`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/appadmin.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/appadmin.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.ics` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.ics`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.jsonp` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.jsonp`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.load` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.load`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/generic.map` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/generic.map`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/layout.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/layout.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/web2py_ajax.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/web2py_ajax.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/applog/applog_layout.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/applog/applog_layout.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/applog/author.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/applog/author.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/applog/index.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/applog/index.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/applog/item.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/applog/item.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/change_password.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/change_password.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/check_domeinen.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/check_domeinen.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/email_footer.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/email_footer.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/items.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/items.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/overdragen.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/overdragen.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/quick_edit.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/quick_edit.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/sticker_beheer.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/sticker_beheer.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/taggem.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/taggem.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/user.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/user.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/default/users.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/default/users.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/organisations/boards.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/organisations/boards.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/organisations/index.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/organisations/index.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/edit.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/edit.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/index.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/index.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/item_dod_rules.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/item_dod_rules.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/item_questions.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/item_questions.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/metadateren.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/metadateren.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/new.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/new.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/tag.html` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/tag.html`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/web2py/apps/workbench/views/workbench/tag_tree.load` & `ontwikkelstraat-1.19.0/web2py/apps/workbench/views/workbench/tag_tree.load`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/.gitignore` & `ontwikkelstraat-1.19.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/pyproject.toml` & `ontwikkelstraat-1.19.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ontwikkelstraat-1.18.1/PKG-INFO` & `ontwikkelstraat-1.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Ontwikkelstraat
-Version: 1.18.1
+Version: 1.19.0
 Summary: Education Warehouse knowledge-sharing setup.
 Project-URL: Documentation, https://github.com/educationwarehouse/ontwikkelstraat#readme
 Project-URL: Issues, https://github.com/educationwarehouse/ontwikkelstraat/issues
 Project-URL: Source, https://github.com/educationwarehouse/ontwikkelstraat
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License: Copyright (c) 2024 Education Warehouse
 License-File: LICENSE.txt
```

