<div id='product-component-024dc854919'></div>
<script type="text/javascript">
//<![CDATA[

/* <BuyButton> */
(function () {
  var scriptURL = 'https://sdks.shopifycdn.com/buy-button/latest/buy-button-storefront.min.js';
  if (window.ShopifyBuy) {
    if (window.ShopifyBuy.UI) {
      ShopifyBuyInit();
    } else {
      loadScript();
    }
  } else {
    loadScript();
  }

  function loadScript() {
    var script = document.createElement('script');
    script.async = true;
    script.src = scriptURL;
    (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(script);
    script.onload = ShopifyBuyInit;
  }

  function ShopifyBuyInit() {
    var client = ShopifyBuy.buildClient({
      domain: 'lilaccityvapor.myshopify.com',
      apiKey: '3eec04fb828fce29f23869caa2b958ca',
      appId: '6',
    });

    ShopifyBuy.UI.onReady(client).then(function (ui) {
      ui.createComponent('product', {
        id: [6124701702],
        node: document.getElementById('product-component-024dc854919'),
        moneyFormat: '${{amount}}',
        options: {
  "product": {
    "buttonDestination": "modal",
    "layout": "vertical",
    "variantId": "all",
    "width": "240px",
    "contents": {
      "img": true,
      "title": true,
      "variantTitle": false,
      "options": false,
      "price": true,
      "description": false,
      "buttonWithQuantity": false,
      "button": true,
      "quantity": false
    },
    "text": {
      "button": "VIEW PRODUCT"
    },
    "styles": {
      "product": {
        "@media (min-width: 601px)": {
          "max-width": "100%",
          "margin-left": "0",
          "margin-bottom": "50px"
        }
      },
      "button": {
        "background-color": "#3d003d",
        "color": "#ffffff",
        "font-family": "Helvetica Neue, sans-serif",
        "font-size": "15px",
        "padding-top": "16px",
        "padding-bottom": "16px",
        "padding-left": "26px",
        "padding-right": "26px",
        "border": "none",
        ":hover": {
          "background-color": "#680068",
          "color": "#ffffff"
        },
        "border-radius": "3px",
        ":focus": {
          "background-color": "#680068"
        }
      },
      "variantTitle": {
        "font-family": "Helvetica Neue, sans-serif",
        "font-size": "14px",
        "color": "#4c4c4c"
      },
      "title": {
        "font-family": "Helvetica Neue, sans-serif",
        "font-weight": "bold",
        "font-size": "18px",
        "color": "#4c4c4c"
      },
      "description": {
        "color": "#4c4c4c",
        "font-size": "14px",
        "font-family": "Helvetica Neue, sans-serif"
      },
      "price": {
        "font-family": "Helvetica Neue, sans-serif",
        "font-size": "14px",
        "color": "#4c4c4c"
      },
      "quantityInput": {
        "font-size": "16px",
        "padding-top": "16px",
        "padding-bottom": "16px",
        "color": "#4c4c4c"
      },
      "compareAt": {
        "font-size": "12px"
      }
    }
  },
  "cart": {
    "contents": {
      "title": true,
      "lineItems": true,
      "footer": true,
      "button": true
    },
    "text": {
      "title": "Cart",
      "total": "Total",
      "notice": "Shipping and discount codes are added at checkout.",
      "button": "CHECKOUT"
    },
    "styles": {
      "button": {
        "background-color": "#3d003d",
        "color": "#ffffff",
        "font-family": "Helvetica Neue, sans-serif",
        "font-size": "16px",
        "padding-top": "16px",
        "padding-bottom": "16px",
        "padding-left": "26px",
        "padding-right": "26px",
        "border": "none",
        ":hover": {
          "background-color": "#680068",
          "color": "#ffffff"
        },
        "border-radius": "3px",
        ":focus": {
          "background-color": "#680068"
        }
      },
      "cart": {
        "background-color": "#000000"
      },
      "footer": {
        "background-color": "#000000"
      },
      "title": {
        "color": "#ffffff"
      },
      "header": {
        "color": "#ffffff"
      },
      "lineItems": {
        "color": "#ffffff"
      },
      "subtotalText": {
        "color": "#ffffff"
      },
      "subtotal": {
        "color": "#ffffff"
      },
      "notice": {
        "color": "#ffffff"
      },
      "currency": {
        "color": "#ffffff"
      },
      "close": {
        ":hover": {
          "color": "#ffffff"
        },
        "color": "#ffffff"
      },
      "emptyCart": {
        "color": "#ffffff"
      }
    }
  },
  "modalProduct": {
    "contents": {
      "img": true,
      "title": true,
      "variantTitle": false,
      "options": true,
      "price": true,
      "description": true,
      "buttonWithQuantity": false,
      "button": true,
      "quantity": false
    },
    "text": {
      "button": "ADD TO CART"
    },
    "styles": {
      "product": {
        "@media (min-width: 601px)": {
          "max-width": "100%",
          "margin-left": "0px",
          "margin-bottom": "0px"
        }
      },
      "button": {
        "background-color": "#3d003d",
        "color": "#ffffff",
        "font-family": "Helvetica Neue, sans-serif",
        "font-size": "15px",
        "padding-top": "16px",
        "padding-bottom": "16px",
        "padding-left": "26px",
        "padding-right": "26px",
        "border": "none",
        ":hover": {
          "background-color": "#680068",
          "color": "#ffffff"
        },
        "border-radius": "3px",
        ":focus": {
          "background-color": "#680068"
        }
      },
      "variantTitle": {
        "font-family": "Helvetica Neue, sans-serif",
        "font-size": "14px",
        "color": "#ffffff"
      },
      "title": {
        "font-family": "Helvetica Neue, sans-serif",
        "font-weight": "bold",
        "font-size": "26px",
        "color": "#ffffff"
      },
      "description": {
        "color": "#ffffff",
        "font-size": "14px",
        "font-family": "Helvetica Neue, sans-serif"
      },
      "price": {
        "font-family": "Helvetica Neue, sans-serif",
        "font-size": "18px",
        "color": "#ff00ff"
      },
      "quantityInput": {
        "font-size": "16px",
        "padding-top": "16px",
        "padding-bottom": "16px",
        "color": "#4c4c4c"
      },
      "compareAt": {
        "font-size": "15px"
      }
    }
  },
  "productSet": {
    "styles": {
      "products": {
        "@media (min-width: 601px)": {
          "margin-left": "-20px"
        }
      }
    }
  },
  "toggle": {
    "styles": {
      "toggle": {
        "font-family": "Helvetica Neue, sans-serif",
        "background-color": "#3d003d",
        ":hover": {
          "background-color": "#680068"
        },
        ":focus": {
          "background-color": "#680068"
        }
      },
      "count": {
        "color": "#ffffff",
        ":hover": {
          "color": "#ffffff"
        }
      },
      "iconPath": {
        "fill": "#ffffff"
      }
    }
  },
  "modal": {
    "styles": {
      "modal": {
        "background-color": "#000000"
      }
    }
  },
  "lineItem": {
    "styles": {
      "variantTitle": {
        "color": "#ffffff"
      },
      "title": {
        "color": "#ffffff"
      },
      "price": {
        "color": "#ffffff"
      },
      "quantity": {
        "color": "#ffffff"
      },
      "quantityIncrement": {
        "color": "#ffffff",
        "border-color": "#ffffff"
      },
      "quantityDecrement": {
        "color": "#ffffff",
        "border-color": "#ffffff"
      },
      "quantityInput": {
        "color": "#ffffff",
        "border-color": "#ffffff"
      }
    }
  },
  "option": {
    "styles": {
      "label": {
        "font-family": "Helvetica Neue, sans-serif",
        "font-weight": "normal",
        "color": "#ffffff"
      },
      "select": {
        "font-family": "Helvetica Neue, sans-serif",
        "font-weight": "normal",
        "color": "#4c4c4c"
      }
    }
  }
}
      });
    });
  }
})();
/* </BuyButton> */
//]]>
</script>
