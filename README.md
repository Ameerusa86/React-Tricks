# React-Tricks

## FULL PAGE SCROLL

## Install

- npm install --save @ap.cx/react-fullpage

## Import

- import { FullPageSections,Fullpage, FullpageNavigation, FullpageSection, }
  from "@ap.cx/react-fullpage";

## Usage

```React JS
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
