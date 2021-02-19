const express = require('express')
const Joi = require('@hapi/joi');
const who = express();

who.post('/auth', async (req, res) => {
    const {error, value} = Joi.object({hwid: Joi.string().required()})
    if(error) return res.status(400).send('Bad request you dumb cunt')
    const Validate_HWID = value.hwid.match(/[0-9,A-z]{8}-[0-9,A-z]{4}-[0-9,A-z]{4}-[0-9,A-z]{4}-[0-9,A-z]{12}/);
    if(!Validate_HWID) return res.status(401).send(`Aw shit looks like you're a dumb cunt`)
    value.hwid = Validate_HWID[0]
    // Add some more code in here you dumb cunt
    // You can use a basic database like Enmap to store shit 
    return res.status(204).send(`Yeah yeah cunt come in`)
})

who.listen(80, () => {
    console.log(`Yeah the little shit is online`)
})
