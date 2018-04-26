## Module AWS.SageMakerRuntime.Types

#### `options`

``` purescript
options :: Options
```

#### `BodyBlob`

``` purescript
newtype BodyBlob
  = BodyBlob String
```

##### Instances
``` purescript
Newtype BodyBlob _
Generic BodyBlob _
Show BodyBlob
Decode BodyBlob
Encode BodyBlob
```

#### `EndpointName`

``` purescript
newtype EndpointName
  = EndpointName String
```

##### Instances
``` purescript
Newtype EndpointName _
Generic EndpointName _
Show EndpointName
Decode EndpointName
Encode EndpointName
```

#### `Header`

``` purescript
newtype Header
  = Header String
```

##### Instances
``` purescript
Newtype Header _
Generic Header _
Show Header
Decode Header
Encode Header
```

#### `InternalFailure`

``` purescript
newtype InternalFailure
  = InternalFailure { "Message" :: Maybe (Message) }
```

<p> Internal failure occurred. </p>

##### Instances
``` purescript
Newtype InternalFailure _
Generic InternalFailure _
Show InternalFailure
Decode InternalFailure
Encode InternalFailure
```

#### `newInternalFailure`

``` purescript
newInternalFailure :: InternalFailure
```

Constructs InternalFailure from required parameters

#### `newInternalFailure'`

``` purescript
newInternalFailure' :: ({ "Message" :: Maybe (Message) } -> { "Message" :: Maybe (Message) }) -> InternalFailure
```

Constructs InternalFailure's fields from required parameters

#### `InvokeEndpointInput`

``` purescript
newtype InvokeEndpointInput
  = InvokeEndpointInput { "EndpointName" :: EndpointName, "Body" :: BodyBlob, "ContentType" :: Maybe (Header), "Accept" :: Maybe (Header) }
```

##### Instances
``` purescript
Newtype InvokeEndpointInput _
Generic InvokeEndpointInput _
Show InvokeEndpointInput
Decode InvokeEndpointInput
Encode InvokeEndpointInput
```

#### `newInvokeEndpointInput`

``` purescript
newInvokeEndpointInput :: BodyBlob -> EndpointName -> InvokeEndpointInput
```

Constructs InvokeEndpointInput from required parameters

#### `newInvokeEndpointInput'`

``` purescript
newInvokeEndpointInput' :: BodyBlob -> EndpointName -> ({ "EndpointName" :: EndpointName, "Body" :: BodyBlob, "ContentType" :: Maybe (Header), "Accept" :: Maybe (Header) } -> { "EndpointName" :: EndpointName, "Body" :: BodyBlob, "ContentType" :: Maybe (Header), "Accept" :: Maybe (Header) }) -> InvokeEndpointInput
```

Constructs InvokeEndpointInput's fields from required parameters

#### `InvokeEndpointOutput`

``` purescript
newtype InvokeEndpointOutput
  = InvokeEndpointOutput { "Body" :: BodyBlob, "ContentType" :: Maybe (Header), "InvokedProductionVariant" :: Maybe (Header) }
```

##### Instances
``` purescript
Newtype InvokeEndpointOutput _
Generic InvokeEndpointOutput _
Show InvokeEndpointOutput
Decode InvokeEndpointOutput
Encode InvokeEndpointOutput
```

#### `newInvokeEndpointOutput`

``` purescript
newInvokeEndpointOutput :: BodyBlob -> InvokeEndpointOutput
```

Constructs InvokeEndpointOutput from required parameters

#### `newInvokeEndpointOutput'`

``` purescript
newInvokeEndpointOutput' :: BodyBlob -> ({ "Body" :: BodyBlob, "ContentType" :: Maybe (Header), "InvokedProductionVariant" :: Maybe (Header) } -> { "Body" :: BodyBlob, "ContentType" :: Maybe (Header), "InvokedProductionVariant" :: Maybe (Header) }) -> InvokeEndpointOutput
```

Constructs InvokeEndpointOutput's fields from required parameters

#### `LogStreamArn`

``` purescript
newtype LogStreamArn
  = LogStreamArn String
```

##### Instances
``` purescript
Newtype LogStreamArn _
Generic LogStreamArn _
Show LogStreamArn
Decode LogStreamArn
Encode LogStreamArn
```

#### `Message`

``` purescript
newtype Message
  = Message String
```

##### Instances
``` purescript
Newtype Message _
Generic Message _
Show Message
Decode Message
Encode Message
```

#### `ModelError`

``` purescript
newtype ModelError
  = ModelError { "Message" :: Maybe (Message), "OriginalStatusCode" :: Maybe (StatusCode), "OriginalMessage" :: Maybe (Message), "LogStreamArn" :: Maybe (LogStreamArn) }
```

<p> Model (owned by the customer in the container) returned an error 500. </p>

##### Instances
``` purescript
Newtype ModelError _
Generic ModelError _
Show ModelError
Decode ModelError
Encode ModelError
```

#### `newModelError`

``` purescript
newModelError :: ModelError
```

Constructs ModelError from required parameters

#### `newModelError'`

``` purescript
newModelError' :: ({ "Message" :: Maybe (Message), "OriginalStatusCode" :: Maybe (StatusCode), "OriginalMessage" :: Maybe (Message), "LogStreamArn" :: Maybe (LogStreamArn) } -> { "Message" :: Maybe (Message), "OriginalStatusCode" :: Maybe (StatusCode), "OriginalMessage" :: Maybe (Message), "LogStreamArn" :: Maybe (LogStreamArn) }) -> ModelError
```

Constructs ModelError's fields from required parameters

#### `ServiceUnavailable`

``` purescript
newtype ServiceUnavailable
  = ServiceUnavailable { "Message" :: Maybe (Message) }
```

<p> Service is unavailable. Try your call again. </p>

##### Instances
``` purescript
Newtype ServiceUnavailable _
Generic ServiceUnavailable _
Show ServiceUnavailable
Decode ServiceUnavailable
Encode ServiceUnavailable
```

#### `newServiceUnavailable`

``` purescript
newServiceUnavailable :: ServiceUnavailable
```

Constructs ServiceUnavailable from required parameters

#### `newServiceUnavailable'`

``` purescript
newServiceUnavailable' :: ({ "Message" :: Maybe (Message) } -> { "Message" :: Maybe (Message) }) -> ServiceUnavailable
```

Constructs ServiceUnavailable's fields from required parameters

#### `StatusCode`

``` purescript
newtype StatusCode
  = StatusCode Int
```

##### Instances
``` purescript
Newtype StatusCode _
Generic StatusCode _
Show StatusCode
Decode StatusCode
Encode StatusCode
```

#### `ValidationError`

``` purescript
newtype ValidationError
  = ValidationError { "Message" :: Maybe (Message) }
```

<p> Inspect your request and try again. </p>

##### Instances
``` purescript
Newtype ValidationError _
Generic ValidationError _
Show ValidationError
Decode ValidationError
Encode ValidationError
```

#### `newValidationError`

``` purescript
newValidationError :: ValidationError
```

Constructs ValidationError from required parameters

#### `newValidationError'`

``` purescript
newValidationError' :: ({ "Message" :: Maybe (Message) } -> { "Message" :: Maybe (Message) }) -> ValidationError
```

Constructs ValidationError's fields from required parameters


