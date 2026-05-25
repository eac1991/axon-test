# Contexto de componente Figma: Button

## Prompt para ChatGPT

Analiza el contexto del elemento de figma que esté en el fichero adjunto.

Revisa:
- Estructura
- Estilo
- Tokens
- Accesibilidad
- Documentación
- ID
- Descripción (alias)

Mantén el contexto del componente durante toda esta conversación para responder preguntas sobre él.

---

## Metadatos

- **Nombre del componente:** Button
- **ID:** `14:1355`
- **Descripción / Alias:** No disponible
- **Archivo Figma:** DS | Components
- **Página:** WIP - Button
- **Exportado:** 2026-05-25T21:02:30.230Z
- **Elementos seleccionados:** 1

---

## Revisión solicitada

- Estructura
- Estilo
- Tokens
- Accesibilidad
- Documentación
- ID
- Descripción (alias)

---

## Resumen estructural

- **Tipo:** INSTANCE
- **Nombre:** Button
- **ID:** `14:1355`
- **Descripción / Alias:** No disponible
- **Dimensiones:** 84 × 40
- **Rol inferido:** button

---

## Datos completos del componente

```json
{
  "exportedAt": "2026-05-25T21:02:30.230Z",
  "fileName": "DS | Components",
  "page": "WIP - Button",
  "selectedComponentName": "Button",
  "selectedComponentId": "14:1355",
  "selectedComponentDescription": null,
  "selectionCount": 1,
  "nodes": [
    {
      "id": "14:1355",
      "name": "Button",
      "type": "INSTANCE",
      "description": null,
      "documentationLinks": null,
      "visible": true,
      "locked": false,
      "width": 84,
      "height": 40,
      "x": 1384,
      "y": 0,
      "rotation": 0,
      "opacity": 1,
      "component": {
        "key": null,
        "remote": null,
        "componentPropertyDefinitions": null,
        "componentPropertyReferences": null,
        "componentProperties": {
          "Icon#24:97": {
            "type": "INSTANCE_SWAP",
            "value": "31:956",
            "preferredValues": [
              {
                "type": "COMPONENT_SET",
                "key": "4bf314b9aaacb89530c7414f708aac9418e2d6a6"
              }
            ]
          },
          "↩︎ Icon#23:0": {
            "type": "BOOLEAN",
            "value": false
          },
          "Kind": {
            "value": "Primary",
            "type": "VARIANT",
            "boundVariables": {}
          },
          "State": {
            "value": "Default",
            "type": "VARIANT",
            "boundVariables": {}
          },
          "Size": {
            "value": "Medium",
            "type": "VARIANT",
            "boundVariables": {}
          },
          "Disabled": {
            "value": "False",
            "type": "VARIANT",
            "boundVariables": {}
          },
          "Danger": {
            "value": "False",
            "type": "VARIANT",
            "boundVariables": {}
          },
          "Label": {
            "value": "True",
            "type": "VARIANT",
            "boundVariables": {}
          }
        },
        "variantProperties": {
          "Kind": "Primary",
          "State": "Default",
          "Size": "Medium",
          "Disabled": "False",
          "Danger": "False",
          "Label": "True"
        }
      },
      "styles": {
        "fills": [
          {
            "type": "SOLID",
            "visible": true,
            "opacity": 1,
            "blendMode": "NORMAL",
            "color": {
              "r": 0,
              "g": 0,
              "b": 0
            },
            "boundVariables": {
              "color": {
                "type": "VARIABLE_ALIAS",
                "id": "VariableID:15bb4db566840e288e76b3707effa17a4415c4fb/24:2"
              }
            }
          }
        ],
        "strokes": [],
        "strokeWeight": 1,
        "effects": [],
        "cornerRadius": 0
      },
      "layout": {
        "constraints": {
          "horizontal": "MIN",
          "vertical": "MIN"
        },
        "layoutMode": "HORIZONTAL",
        "primaryAxisSizingMode": "AUTO",
        "counterAxisSizingMode": "FIXED",
        "itemSpacing": 8,
        "paddingTop": 8,
        "paddingRight": 24,
        "paddingBottom": 8,
        "paddingLeft": 24
      },
      "text": {
        "characters": null,
        "fontSize": null,
        "fontName": null,
        "lineHeight": null,
        "letterSpacing": null,
        "textAlignHorizontal": null,
        "textAlignVertical": null
      },
      "tokens": {
        "boundVariables": {
          "itemSpacing": {
            "type": "VARIABLE_ALIAS",
            "id": "VariableID:8cbc44f61b5af84ca4112c8486d845255cb5b8db/19:133"
          },
          "paddingLeft": {
            "type": "VARIABLE_ALIAS",
            "id": "VariableID:21597c53c7bc558f36640be95470e070aa051122/19:130"
          },
          "paddingTop": {
            "type": "VARIABLE_ALIAS",
            "id": "VariableID:8cbc44f61b5af84ca4112c8486d845255cb5b8db/19:133"
          },
          "paddingRight": {
            "type": "VARIABLE_ALIAS",
            "id": "VariableID:21597c53c7bc558f36640be95470e070aa051122/19:130"
          },
          "paddingBottom": {
            "type": "VARIABLE_ALIAS",
            "id": "VariableID:8cbc44f61b5af84ca4112c8486d845255cb5b8db/19:133"
          },
          "height": {
            "type": "VARIABLE_ALIAS",
            "id": "VariableID:8fd58ba3e823ff5a1bf850da096b632c0ca82f62/19:147"
          },
          "fills": [
            {
              "type": "VARIABLE_ALIAS",
              "id": "VariableID:15bb4db566840e288e76b3707effa17a4415c4fb/24:2"
            }
          ]
        },
        "explicitVariableModes": {},
        "resolvedVariableModes": {
          "VariableCollectionId:036b3044e918e51a8c74d11a2ea4636287524f79/4:217": "4:0",
          "VariableCollectionId:cb552568589a268659ee9444ed824006bdb54b27/19:129": "4:1",
          "VariableCollectionId:600c7d9bb1727a9944be116e9ab29265c89b57ad/23:270": "2:0"
        },
        "fillStyleId": "",
        "strokeStyleId": "",
        "effectStyleId": "",
        "textStyleId": null
      },
      "accessibilityHints": {
        "inferredRole": "button",
        "hasVisibleText": false,
        "width": 84,
        "height": 40
      },
      "children": [
        {
          "id": "I14:1355;23:219",
          "name": "Icon",
          "type": "FRAME",
          "description": null,
          "documentationLinks": null,
          "visible": false,
          "locked": false,
          "width": 20,
          "height": 20,
          "x": 24,
          "y": 10,
          "rotation": 0,
          "opacity": 1,
          "component": {
            "key": null,
            "remote": null,
            "componentPropertyDefinitions": null,
            "componentPropertyReferences": {
              "visible": "↩︎ Icon#23:0"
            },
            "componentProperties": null,
            "variantProperties": null
          },
          "styles": {
            "fills": [],
            "strokes": [],
            "strokeWeight": 1,
            "effects": [],
            "cornerRadius": 0
          },
          "layout": {
            "constraints": {
              "horizontal": "MIN",
              "vertical": "MIN"
            },
            "layoutMode": "HORIZONTAL",
            "primaryAxisSizingMode": "AUTO",
            "counterAxisSizingMode": "AUTO",
            "itemSpacing": 10,
            "paddingTop": 0,
            "paddingRight": 0,
            "paddingBottom": 0,
            "paddingLeft": 0
          },
          "text": {
            "characters": null,
            "fontSize": null,
            "fontName": null,
            "lineHeight": null,
            "letterSpacing": null,
            "textAlignHorizontal": null,
            "textAlignVertical": null
          },
          "tokens": {
            "boundVariables": {},
            "explicitVariableModes": {},
            "resolvedVariableModes": {
              "VariableCollectionId:600c7d9bb1727a9944be116e9ab29265c89b57ad/23:270": "2:0"
            },
            "fillStyleId": "",
            "strokeStyleId": "",
            "effectStyleId": "",
            "textStyleId": null
          },
          "accessibilityHints": {
            "inferredRole": "icon",
            "hasVisibleText": false,
            "width": 20,
            "height": 20
          },
          "children": [
            {
              "id": "I14:1355;23:220",
              "name": "Information",
              "type": "INSTANCE",
              "description": null,
              "documentationLinks": null,
              "visible": true,
              "locked": false,
              "width": 20,
              "height": 20,
              "x": 0,
              "y": 0,
              "rotation": 0,
              "opacity": 1,
              "component": {
                "key": null,
                "remote": null,
                "componentPropertyDefinitions": null,
                "componentPropertyReferences": {
                  "mainComponent": "Icon#24:97"
                },
                "componentProperties": {
                  "Filled": {
                    "value": "False",
                    "type": "VARIANT",
                    "boundVariables": {}
                  }
                },
                "variantProperties": {
                  "Filled": "False"
                }
              },
              "styles": {
                "fills": [],
                "strokes": [],
                "strokeWeight": 1,
                "effects": [],
                "cornerRadius": 0
              },
              "layout": {
                "constraints": {
                  "horizontal": "MIN",
                  "vertical": "MIN"
                },
                "layoutMode": "NONE",
                "primaryAxisSizingMode": "AUTO",
                "counterAxisSizingMode": "FIXED",
                "itemSpacing": 0,
                "paddingTop": 0,
                "paddingRight": 0,
                "paddingBottom": 0,
                "paddingLeft": 0
              },
              "text": {
                "characters": null,
                "fontSize": null,
                "fontName": null,
                "lineHeight": null,
                "letterSpacing": null,
                "textAlignHorizontal": null,
                "textAlignVertical": null
              },
              "tokens": {
                "boundVariables": {},
                "explicitVariableModes": {},
                "resolvedVariableModes": {
                  "VariableCollectionId:600c7d9bb1727a9944be116e9ab29265c89b57ad/23:270": "2:0"
                },
                "fillStyleId": "",
                "strokeStyleId": "",
                "effectStyleId": "",
                "textStyleId": null
              },
              "accessibilityHints": {
                "inferredRole": "unknown",
                "hasVisibleText": false,
                "width": 20,
                "height": 20
              },
              "children": [
                {
                  "id": "I14:1355;23:220;16:423",
                  "name": "Shape",
                  "type": "VECTOR",
                  "description": null,
                  "documentationLinks": null,
                  "visible": true,
                  "locked": false,
                  "width": 16,
                  "height": 16,
                  "x": 2,
                  "y": 2,
                  "rotation": 0,
                  "opacity": 1,
                  "component": {
                    "key": null,
                    "remote": null,
                    "componentPropertyDefinitions": null,
                    "componentPropertyReferences": {},
                    "componentProperties": null,
                    "variantProperties": null
                  },
                  "styles": {
                    "fills": [
                      {
                        "type": "SOLID",
                        "visible": true,
                        "opacity": 1,
                        "blendMode": "NORMAL",
                        "color": {
                          "r": 1,
                          "g": 1,
                          "b": 1
                        },
                        "boundVariables": {
                          "color": {
                            "type": "VARIABLE_ALIAS",
                            "id": "VariableID:01cf4c070149d583e71b0c20ed775dd8e279e87b/23:293"
                          }
                        }
                      }
                    ],
                    "strokes": [],
                    "strokeWeight": 1,
                    "effects": [],
                    "cornerRadius": 0
                  },
                  "layout": {
                    "constraints": {
                      "horizontal": "SCALE",
                      "vertical": "SCALE"
                    },
                    "layoutMode": null,
                    "primaryAxisSizingMode": null,
                    "counterAxisSizingMode": null,
                    "itemSpacing": null,
                    "paddingTop": null,
                    "paddingRight": null,
                    "paddingBottom": null,
                    "paddingLeft": null
                  },
                  "text": {
                    "characters": null,
                    "fontSize": null,
                    "fontName": null,
                    "lineHeight": null,
                    "letterSpacing": null,
                    "textAlignHorizontal": null,
                    "textAlignVertical": null
                  },
                  "tokens": {
                    "boundVariables": {
                      "fills": [
                        {
                          "type": "VARIABLE_ALIAS",
                          "id": "VariableID:01cf4c070149d583e71b0c20ed775dd8e279e87b/23:293"
                        }
                      ]
                    },
                    "explicitVariableModes": {},
                    "resolvedVariableModes": {
                      "VariableCollectionId:600c7d9bb1727a9944be116e9ab29265c89b57ad/23:270": "2:0"
                    },
                    "fillStyleId": "",
                    "strokeStyleId": "",
                    "effectStyleId": "",
                    "textStyleId": null
                  },
                  "accessibilityHints": {
                    "inferredRole": "unknown",
                    "hasVisibleText": false,
                    "width": 16,
                    "height": 16
                  },
                  "children": []
                }
              ]
            }
          ]
        },
        {
          "id": "I14:1355;9:194",
          "name": "Label",
          "type": "TEXT",
          "description": null,
          "documentationLinks": null,
          "visible": true,
          "locked": false,
          "width": 36,
          "height": 22,
          "x": 24,
          "y": 9,
          "rotation": 0,
          "opacity": 1,
          "component": {
            "key": null,
            "remote": null,
            "componentPropertyDefinitions": null,
            "componentPropertyReferences": {},
            "componentProperties": null,
            "variantProperties": null
          },
          "styles": {
            "fills": [
              {
                "type": "SOLID",
                "visible": true,
                "opacity": 1,
                "blendMode": "NORMAL",
                "color": {
                  "r": 1,
                  "g": 1,
                  "b": 1
                },
                "boundVariables": {
                  "color": {
                    "type": "VARIABLE_ALIAS",
                    "id": "VariableID:01cf4c070149d583e71b0c20ed775dd8e279e87b/23:293"
                  }
                }
              }
            ],
            "strokes": [],
            "strokeWeight": 1,
            "effects": [],
            "cornerRadius": null
          },
          "layout": {
            "constraints": {
              "horizontal": "MIN",
              "vertical": "MIN"
            },
            "layoutMode": null,
            "primaryAxisSizingMode": null,
            "counterAxisSizingMode": null,
            "itemSpacing": null,
            "paddingTop": null,
            "paddingRight": null,
            "paddingBottom": null,
            "paddingLeft": null
          },
          "text": {
            "characters": "Label",
            "fontSize": 14,
            "fontName": {
              "family": "Inter",
              "style": "Regular"
            },
            "lineHeight": {
              "unit": "PIXELS",
              "value": 22
            },
            "letterSpacing": {
              "unit": "PIXELS",
              "value": 0
            },
            "textAlignHorizontal": "LEFT",
            "textAlignVertical": "TOP"
          },
          "tokens": {
            "boundVariables": {
              "fills": [
                {
                  "type": "VARIABLE_ALIAS",
                  "id": "VariableID:01cf4c070149d583e71b0c20ed775dd8e279e87b/23:293"
                }
              ],
              "letterSpacing": [
                {
                  "type": "VARIABLE_ALIAS",
                  "id": "VariableID:10a942f64197a33acf331c93cd67df25ec55a095/19:189"
                }
              ],
              "fontSize": [
                {
                  "type": "VARIABLE_ALIAS",
                  "id": "VariableID:19fc85db9d12a612f0c5cd9e2c269f240ba7c522/19:165"
                }
              ],
              "fontFamily": [
                {
                  "type": "VARIABLE_ALIAS",
                  "id": "VariableID:2aa7e51c3e789aa958a03f1b3d3ec3c7d435298c/19:151"
                }
              ],
              "lineHeight": [
                {
                  "type": "VARIABLE_ALIAS",
                  "id": "VariableID:44d590734fb9895f2ac150048034f2d0651a6d58/19:174"
                }
              ],
              "fontWeight": [
                {
                  "type": "VARIABLE_ALIAS",
                  "id": "VariableID:3f6d3eb3aaae67632aa71affc1425e4007c05a42/6:7"
                }
              ]
            },
            "explicitVariableModes": {},
            "resolvedVariableModes": {
              "VariableCollectionId:036b3044e918e51a8c74d11a2ea4636287524f79/4:217": "4:0",
              "VariableCollectionId:cb552568589a268659ee9444ed824006bdb54b27/19:129": "4:1",
              "VariableCollectionId:600c7d9bb1727a9944be116e9ab29265c89b57ad/23:270": "2:0"
            },
            "fillStyleId": "",
            "strokeStyleId": "",
            "effectStyleId": "",
            "textStyleId": "S:7274806b011ae418173e29868ce1e276d2e107fd,19:196"
          },
          "accessibilityHints": {
            "inferredRole": "unknown",
            "hasVisibleText": true,
            "width": 36,
            "height": 22
          },
          "children": []
        }
      ]
    }
  ]
}
```
