# React-Tricks

## FULL PAGE SCROLL

## Install

- npm install --save @ap.cx/react-fullpage

## Import

- import { FullPageSections,Fullpage, FullpageNavigation, FullpageSection, }
  from "@ap.cx/react-fullpage";

## Usage

```Full Page Scroller
<!-- Example Code -->
const FullPageScroll = () => {
return (
<Fullpage>
<FullpageNavigation />
<FullPageSections>
<FullpageSection style={{ height: "100vh" }}> \<Page 1 />
</FullpageSection>
<FullpageSection style={{ height: "100vh" }}>
<Page 2 />
</FullpageSection>
<FullpageSection style={{ height: "100vh" }}>
<Page 3/>
</FullpageSection>
</FullPageSections>
</Fullpage> ); };

export default FullPageScroll;
```

```Random Number Counter
import React, { useEffect, useState } from "react";

const Counter = (props) => {
  const { startCount } = props;
  const [stopCount, setStopCount] = useState(0);
  const [count, setCount] = useState(startCount);

  useEffect(() => {
    if (count === stopCount) {
      return;
    }

    const intervalId = setInterval(() => {
      setCount((prevCount) => prevCount + 1);
    }, 25);

    return () => clearInterval(intervalId);
  }, [count, stopCount]);

  useEffect(() => {
    const randomStopCount = Math.floor(Math.random() * 100) + 1;
    setStopCount(randomStopCount);
  }, []);

  return <div>{count}</div>;
};

export default Counter;
```
