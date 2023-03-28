## Video views indicator

<br/>

<div class="grid grid-cols-2 gap-4">
<div>
Get views for the video with `VIDEO_ID` identifier:

```sh
$ curl \
    http://localhost:8100/api/v1/video/VIDEO_ID/views
```

Example response:

```json
{
  "total": 73,
  "daily_views": [
    {"day": "2023-02-18", "views": 3},
    {"day": "2023-02-19", "views": 3},
    // [...]
    {"day": "2023-03-17", "views": 5}
  ]
}
```
</div>
<div>
`DailyViews` React component example integration:

```typescript
// web.tsx
import type { ReactElement } from "react";
import type { NextPageWithLayout } from "./_app";

import { DailyViews } from "ui";

const Web: NextPageWithLayout = () => {
  const videoIds = [
    "VIDEO_ID_01",
    "VIDEO_ID_02",
  ];
  return (
    <>
      <DailyViews videoIds={videoIds} />
    </>
  );
};

export default Web;
```

</div>
</div>
