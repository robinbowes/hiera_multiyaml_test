Testing functionality of hiera-multiyaml

ensure both hiera and hiera-multiyaml are installed.

hiera -c hiera.yaml role
=> returns: two::common

hiera -c hiera.yaml groups
=> returns: ["two common item 1", "two common item 2"]

ie. the items in the 2nd datadir replace those in the 1st.
