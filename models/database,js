const pg = require('pg');
const connectionString = process.env.DATABASE_URL || 'postgres://postgres:1234@localhost:5432/bdcomercial';

const client = new pg.Client(connectionString);
client.connect();
const query = client.query(
  'select * from usuario');
query.on('end', () => { client.end(); });