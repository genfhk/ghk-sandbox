# sandbox
### heading?
#### heading?
h1. Wikifier RT

h1. +Quick Links+

h2. Metadata

{color:#000000}NYPL AMI metadata schema{color}{color:#000000} {color}[https://github.com/NYPL/ami-metadata]{color:#000000} {color}{color:#000000} {color}

{color:#000000}NYPL AMI metadata schema validator{color}{color:#000000} {color}[https://github.com/nypl/ami-metadata]{color:#000000} {color}

h2. File Packaging

{color:#000000}BagIt {color}{color:#000000} {color} {color:#1155CC}[https://tools.ietf.org/html/draft-kunze-bagit-13|https://tools.ietf.org/html/draft-kunze-bagit-13.]{color}


|Component | Formats | Note|
| --- | ----| ----|
| Volume: v## | <ul><li>A Volume is one video or audio object in a set of objects, when that set has been assigned a single primary identifier (i.e. NYPL classmark)</li></ul> | Audio and video|
| Face: f## | <ul><li>A Face is a stream or track, or a group of streams or tracks which play synchronously, within an audio object. Every audio object has at least one Face.</li></ul> | Audio only|
| Region: r## | <ul><li>A Region is a subdivision of a Face.</li><li>Regions are most often defined by a required change in playback characteristics (speed, EQ, track configuration, etc) of an object's Face.</li><li>This is rarely used for video objects.</li></ul> | Audio and video|
| Stream: s## | <ul><li>The Stream element is used to describe multi-track and multi-channel audio objects only.</li><li>Streams are one-channel or interleaved two-channel audio streams which comprise a multi-channel or multi-track audio object.</li></ul> | Audio only|
| Part: p## | <ul><li>The part element is used when digitization of a single face of an audio or video object requires interruption because the size of the resulting file would exceed technical limits if captured all at once.</li><li>The part element may also be used when a single tape contains sections of content that are each given different unique identifiers (each section would be a distinct Part).</li></ul> | Audio and video|
| Take: t## | <ul><li>A Take is an alternate preservation capture of an entire object face, produced with alternate playback characteristics in order to compare quality or results (stylus, EQ, speed, etc.). Rare occurrence.</li></ul> | Audio only|
