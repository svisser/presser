#Presser v0.1

This is a simple library that attempts to extract the data for a vine from a given vine.co URL. Its a little rough and ready, and given that Vine can change their page design at any time, cannot be guaranteed to work.

However, here is the example usage.
    from presser.presser import Presser
    press = Presser()

    #For a vine id
    vine = press.get_data_for_vine_id("OBiwWuBm0Eg")

    #For a vine url
    vine = press.get_data_for_vine_from_url("https://vine.co/v/OBiwWuBm0Eg")

    vine.keys()
    vine["avatarUrl"]

##Warning

Vine does not allow scraping, so please do not use this in an automated fashion, but it should be okay that if a user were to go to the url, then you can automate the extraction.

So if you were to get the user to paste the vine url and extract the data, then you should be okay.

If you try to do large batches of vine urls for extraction in a short period of time, then you will probably annoy Vine. Don't do this please.