### Documentação para o App Ionic

#### Subdomain e Domain

    GET	/subdomains/1.json
    GET	/domains/1.json

Domain Field

    tag_location: []

Subdomain Field

    :button_text_client,
    :button_text_service,
    :cover,
    :primary_colour,
    :secundary_colour,
    :contrast_colour,
    :logo,
    :find_clients,
    :find_professional,
    :publications_wall,
    :deepening_placeholder,
    :custom_placeholder,
    :target_placeholder,
    :cards_wall,
    tag_speciality: [],
    tag_target: [],
    tag_custom: [],
    tag_publication_kind: [],
    tag_deepening: []

#### Publication

    POST	/publications.json
    GET	    /publications/:id.json
    PATCH	/publications/:id.json
    PUT	    /publications/:id.json
    DELETE	/publications/:id.json
    	
    GET	    /publications/from-user/:user_id.json
    GET	    /publications/from-subdomain/1.json

Fields

    :title,
    :description,
    :image,
    :is_published,
    :subdomain_id = 1
    :domain_id = 1
    :profile_id = Get from current_user
    tag_publication_kind: [] = Get from subdomain
    user_id = current_user

#### Upload de imagens

No rails é utilizado o carrierwave para upload.

#### Cards

    POST	/cards.json
    GET	    /cards/:id.json
    PATCH	/cards/:id.json
    PUT   	/cards/:id.json
    DELETE	/cards/:id.json
     	 
    GET  	/cards/from-user/:user_id.json
    GET	    /cards/from-subdomain/1.json


#### Profile

    POST	/profiles.json
    GET	    /profiles/:id.json
    PATCH	/profiles/:id.json
    PUT	    /profiles/:id.json
    DELETE	/profiles/:id.json
    GET	    /profiles/from-user/:user_id.json
    GET	    /profiles/main/:user_id.json

