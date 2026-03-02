# Conversation Intelligence Data Sources

## Gong

### Connection
- API Key: [from Gong Settings]
- Access Key: [from Gong Settings]
- Base URL: `https://api.gong.io`

### Key Endpoints

**Calls:**
```javascript
GET /v2/calls
Parameters:
- workspaceId: [workspace]
- fromDateTime: [ISO date]
- toDateTime: [ISO date]
- participants.email: [email]
```

**Transcripts:**
```javascript
GET /v2/calls/{callId}/transcript
Returns: Timestamped transcript with speaker identification
```

**Insights:**
```javascript
GET /v2/calls/{callId}/insights
Returns: Key moments, action items, topics
```

### Key Queries

**Calls by Account:**
```javascript
const calls = await gong.calls.list({
  participants: accountContacts,
  fromDateTime: startDate,
  toDateTime: endDate
});
```

**Extract Quotes:**
```javascript
const transcript = await gong.transcripts.get(callId);
const quotes = extractQuotes(transcript, keywords);
```

## Chorus

### Connection
- API Key: [from Chorus Settings]
- Base URL: `https://api.chorus.ai`

### Key Endpoints
Similar structure to Gong.

## Key Data Extracted

### From Transcripts
- Pain points mentioned
- Feature requests
- Use cases discussed
- Competitive mentions
- Objections raised
- Decision criteria

### From Insights
- Action items
- Next steps
- Key moments
- Topic summaries

### For QBRs
- Customer quotes (verbatim)
- Implemented use cases
- Expansion signals
- Sentiment indicators
