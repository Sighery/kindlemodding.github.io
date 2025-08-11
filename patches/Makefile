.PHONY: patch-ads
patch-ads:
	git checkout -b temp-revert && \
	git revert --no-commit 7276ba2faa6f06ee9f8cbc3b9e5372330eda1e50 && \
	git revert --no-commit 56b68dfc29e110a15d28ee415a7abea9352a89bb && \
	git revert --no-commit 701e90c9f2043bb72e6239e6556e7136ebfc7a50 && \
	git revert --no-commit efedee4905945344dc657f433dbc907a4621f892 && \
	git revert --no-commit 537370c71f8fbdb391eb0d139c48c372d2eea314 && \
	git revert --no-commit e192612697a70d216aa632aa91327aa628d192f0 && \
	git revert --no-commit f374e8a637b6dabad77a6a8547dfbde35f885ec5 && \
	git revert --no-commit 035350c27ab907d208b029699ce8ac37f52a6db4 && \
	git revert --no-commit f445dc526d6fefdc7ce7dabe14fd0a68dc6a0ae7 && \
	git revert --no-commit a1fc86ccb7411d8728b97a08d70936a205f354f0 && \
	git revert --no-commit 971bdef26ed3fd8e9e35226e43a51d199a49eae0 && \
	git revert --no-commit fc89caa1232accf917a5c9a3048265fc6310dc95 && \
	git revert --no-commit 0022a6884848800cf1b447da0ee4237592e674cd && \
	git revert --no-commit 45f93e10d5ea32d3486d9550aabbf3753dd010b7 && \
	git revert --no-commit 05057b5f879f888c5b1c238c23a5fd42773c8243 && \
	git revert --no-commit df7d0cd3db67cddb337ce7685d12996bfa5d7c04 && \
	git revert --no-commit 2e181e6c1189ba5427cb1355aad4e65045f7a2dc && \
	git revert --no-commit b96e777c31d970169ef6f98229fee838855248dd && \
	git diff --cached > 01-ads.patch && \
	git revert --abort && \
	git checkout main && git branch -D temp-revert

.PHONY: generate-patches
generate-patches: patch-ads
