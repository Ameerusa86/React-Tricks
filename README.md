# React-Tricks
##React Full Page Scroll import React from "react"; import { FullPageSections,
Fullpage, FullpageNavigation, FullpageSection, } from "@ap.cx/react-fullpage";

<!-- Import Pages -->

import Home from "./Pages/Home/Home"; import Products from
"./Pages/Products/Products";

const FullPageScroll = () => { return ( <Fullpage> <FullpageNavigation />
<FullPageSections> <FullpageSection style={{ height: "100vh" }}> <Home />
</FullpageSection> <FullpageSection style={{ height: "100vh" }}> <Products />
</FullpageSection> <FullpageSection style={{ height: "100vh" }}> <h1>Section
3</h1> </FullpageSection> </FullPageSections> </Fullpage> ); };

export default FullPageScroll;
