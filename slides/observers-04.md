##  Contrived Example (model)

    name: DS.attr('string')
    company: DS.attr('string')
    # Fancy String Interpolation thank ES6
    sui: ( -> `${this.get('company')}\${this.get('name')}`).property('name', 'company')
    drawUserPicture: (->
      # My REALLY complicated function that takes a couple seconds to run
    ).observes('sui', 'name', 'company')
