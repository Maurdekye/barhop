##Documentation of the Barhop Model 

    locate_bars(position, radius, limit=50)
    '''
    inputs:
      positon: longitude, latitude tuple of the center location to search from
      radius: radius in kilometers to search in around the position
      limit: maximum number of bars to return in a list
    returns: list of dictionaries in the form of: 
      [
        {
        	location: (<longitude>,<latitude>), 
          id: <bar id>
        }
      ]
    '''

    get_bar_info(bar_id)
    '''
    inputs:
      bar_id: bar id representing the bar that information is desired of
    returns: dictionary in the form of:
      {
        name: <name of bar>,
        address: <address of bar>,
        phone_number: <phone number of bar>,
        rating: <average bar rating>
      }
    '''

    get_reservations(user_id)
    '''
    inputs:
      user_id: id of user to retrieve reservations of
    returns: list in the form:
      [
        <id of specific reservation>
      ]
    '''

    get_reservation_info(reservation_id)
    '''
    inputs:
      reservation_id: id of reservation to retrieve information about
    returns: dictionary in the form:
      {
        bar_id: <id of bar reservation is at>,
        date: <date of reservation>,
        time: <time of reservation>,
        length: <duration of reservation, in minutes>
      }
    '''