## Objects

<dl>
<dt><a href="#Definitions">Definitions</a> : <code>object</code></dt>
<dd></dd>
<dt><a href="#helperFunctions">helperFunctions</a> : <code>object</code></dt>
<dd></dd>
<dt><a href="#launchFunctions">launchFunctions</a> : <code>object</code></dt>
<dd></dd>
</dl>

<a name="Definitions"></a>

## Definitions : <code>object</code>
**Kind**: global namespace  
<a name="helperFunctions"></a>

## helperFunctions : <code>object</code>
**Kind**: global namespace  

* [helperFunctions](#helperFunctions) : <code>object</code>
    * [.stringToSHA256(str)](#helperFunctions.stringToSHA256) ⇒
    * [.stringToByteBuffer(str)](#helperFunctions.stringToByteBuffer) ⇒
    * [.intFromBytes(bytearray)](#helperFunctions.intFromBytes) ⇒
    * [.roundFloat(float)](#helperFunctions.roundFloat) ⇒
    * [.getTime(full)](#helperFunctions.getTime) ⇒
    * [.projectAudit()](#helperFunctions.projectAudit)
    * [.crc32(str)](#helperFunctions.crc32) ⇒
    * [.parsedJsonStringsToInt(object)](#helperFunctions.parsedJsonStringsToInt) ⇒
    * [.degreesToRadians(deg)](#helperFunctions.degreesToRadians)
    * [.radiansToDegrees(rad)](#helperFunctions.radiansToDegrees)
    * [.milesToKilometers(miles)](#helperFunctions.milesToKilometers)
    * [.kilometersToMiles(kilometers)](#helperFunctions.kilometersToMiles)
    * [.bytesToHexString(data, length)](#helperFunctions.bytesToHexString)
    * [.arrayRandom(arr)](#helperFunctions.arrayRandom)
    * [.capitalizeString(str)](#helperFunctions.capitalizeString)
    * [.generateOrdinal(i)](#helperFunctions.generateOrdinal) ⇒
    * [.removeMarkdownTags(str)](#helperFunctions.removeMarkdownTags) ⇒
    * [.camelCase(str)](#helperFunctions.camelCase) ⇒

<a name="helperFunctions.stringToSHA256"></a>

### helperFunctions.stringToSHA256(str) ⇒
**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: ByteBuffer containing SHA256 encoded str  

| Param | Type |
| --- | --- |
| str | <code>string</code> | 

<a name="helperFunctions.stringToByteBuffer"></a>

### helperFunctions.stringToByteBuffer(str) ⇒
**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: Byte Array containing encoded str  

| Param | Type |
| --- | --- |
| str | <code>string</code> | 

<a name="helperFunctions.intFromBytes"></a>

### helperFunctions.intFromBytes(bytearray) ⇒
**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: Decoded 64-bit Floating Point number  

| Param | Type |
| --- | --- |
| bytearray | <code>bytearray</code> | 

<a name="helperFunctions.roundFloat"></a>

### helperFunctions.roundFloat(float) ⇒
Useful for rounding single-precision floats (such as those encoded in a Java application)

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: Number rounded to the 100ths place.  

| Param | Type |
| --- | --- |
| float | <code>number</code> | 

<a name="helperFunctions.getTime"></a>

### helperFunctions.getTime(full) ⇒
**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: Formatted string time  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| full | <code>boolean</code> | <code>false</code> | Whether or not function returns seconds. default: false. |

<a name="helperFunctions.projectAudit"></a>

### helperFunctions.projectAudit()
Iterates over all files (excluding node_modules and the like) to determine the (roughly estimated) number of lines of code in a given projectAsynchronous

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
<a name="helperFunctions.crc32"></a>

### helperFunctions.crc32(str) ⇒
Generates a crc32 checksum from a string

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: crc32 checksum number  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | The stringified data to be converted. |

<a name="helperFunctions.parsedJsonStringsToInt"></a>

### helperFunctions.parsedJsonStringsToInt(object) ⇒
Takes a parsed JSON object which contains numbers read as strings and converts those strings to numbers.e.g. userID: "1234" would become userID: 1234.Also has the nasty tendency to turn empty arrays into zeroes.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: Object with numbers, rather than strings.  

| Param | Type | Description |
| --- | --- | --- |
| object | <code>object</code> | The stringified data to be converted. |

<a name="helperFunctions.degreesToRadians"></a>

### helperFunctions.degreesToRadians(deg)
Converts degrees to radians. Simple as.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  

| Param | Type |
| --- | --- |
| deg | <code>number</code> | 

<a name="helperFunctions.radiansToDegrees"></a>

### helperFunctions.radiansToDegrees(rad)
Converts radians to degrees. Simple as.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  

| Param | Type |
| --- | --- |
| rad | <code>number</code> | 

<a name="helperFunctions.milesToKilometers"></a>

### helperFunctions.milesToKilometers(miles)
Converts miles to kilometers. Simple as.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  

| Param | Type |
| --- | --- |
| miles | <code>number</code> | 

<a name="helperFunctions.kilometersToMiles"></a>

### helperFunctions.kilometersToMiles(kilometers)
Converts kilometers to miles. Simple as.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  

| Param | Type |
| --- | --- |
| kilometers | <code>number</code> | 

<a name="helperFunctions.bytesToHexString"></a>

### helperFunctions.bytesToHexString(data, length)
Converts a byte array into a hexadecimal string.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| data | <code>bytearray</code> |  | Data to be encoded |
| length | <code>number</code> | <code>32</code> | The maximum number of bytes which will be read (left justified). Default: 32. |

<a name="helperFunctions.arrayRandom"></a>

### helperFunctions.arrayRandom(arr)
Selects a pseudorandom value from the provided array.Because I was sick of typing 'Math.' 200 times.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  

| Param | Type | Description |
| --- | --- | --- |
| arr | <code>array</code> | Array to be selected from. |

<a name="helperFunctions.capitalizeString"></a>

### helperFunctions.capitalizeString(str)
Capitalizes a given string.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | String to be capitalized |

<a name="helperFunctions.generateOrdinal"></a>

### helperFunctions.generateOrdinal(i) ⇒
Generates an ordinal suffix for a number.e.g. 1 becomes 1st, 9 becomes 9th.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: The number concatenated with its ordinal.  

| Param | Type | Description |
| --- | --- | --- |
| i | <code>number</code> | The number for which an ordinal will be generated. |

<a name="helperFunctions.removeMarkdownTags"></a>

### helperFunctions.removeMarkdownTags(str) ⇒
Coarsely removes markdown tags from a string.e.g. *Hello __world__* becomes Hello world

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: The number without markdown tags  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | The string with Markdown formatting |

<a name="helperFunctions.camelCase"></a>

### helperFunctions.camelCase(str) ⇒
Formats a string to camelCasee.g. Hello World becomes helloWorld.

**Kind**: static method of [<code>helperFunctions</code>](#helperFunctions)  
**Returns**: camelCase string  

| Param | Type |
| --- | --- |
| str | <code>string</code> | 

<a name="launchFunctions"></a>

## launchFunctions : <code>object</code>
**Kind**: global namespace  

* [launchFunctions](#launchFunctions) : <code>object</code>
    * [.stringFromData(bb)](#launchFunctions.stringFromData) ⇒
    * [.getStringData(str)](#launchFunctions.getStringData) ⇒
    * [.getStringDataSize(str)](#launchFunctions.getStringDataSize) ⇒
    * [.sanitizeName(str)](#launchFunctions.sanitizeName) ⇒
    * [.cleanJSONGameSave(json)](#launchFunctions.cleanJSONGameSave) ⇒

<a name="launchFunctions.stringFromData"></a>

### launchFunctions.stringFromData(bb) ⇒
Reads a Short at the provided ByteBuffer's offset, reads a string of the length denoted by the read short.This DOES iterate the ByteBuffer in the namespace where the function is called.

**Kind**: static method of [<code>launchFunctions</code>](#launchFunctions)  
**Returns**: The string which was read.  

| Param | Type | Description |
| --- | --- | --- |
| bb | <code>ByteBuffer</code> | The ByteBuffer from which the string will be read. |

<a name="launchFunctions.getStringData"></a>

### launchFunctions.getStringData(str) ⇒
Converts a string to a ByteBuffer containing a short (representing the length of the converted string), followed by the converted string.

**Kind**: static method of [<code>launchFunctions</code>](#launchFunctions)  
**Returns**: ByteArray  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | The string which will be converted. |

<a name="launchFunctions.getStringDataSize"></a>

### launchFunctions.getStringDataSize(str) ⇒
Returns the byte-size of a short (representing the length of the string), followed by a byte-encoded string

**Kind**: static method of [<code>launchFunctions</code>](#launchFunctions)  
**Returns**: Number  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | The string which will be measured. |

<a name="launchFunctions.sanitizeName"></a>

### launchFunctions.sanitizeName(str) ⇒
Sanitized the given name for profanity, as well as dangerous characters. Not currently functional.

**Kind**: static method of [<code>launchFunctions</code>](#launchFunctions)  
**Returns**: The sanitized string.  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | The string which will be sanitized. |

<a name="launchFunctions.cleanJSONGameSave"></a>

### launchFunctions.cleanJSONGameSave(json) ⇒
Cleans coarsely converted JSON game save (from XML) for use in Counterforce.This is an ultra-specific function for Counterforce.

**Kind**: static method of [<code>launchFunctions</code>](#launchFunctions)  
**Returns**: Cleaned object.  

| Param | Type | Description |
| --- | --- | --- |
| json | <code>object</code> | The parsed JSON object. |

