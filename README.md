
# DVD Rental Database Analysis for SQL Project

In this project, we look into the DVD Rental Database and investigate a total of 10 queries in order to generate some insightful business conclusions.

![App Screenshot](data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxMTEhUTExMWFhUXGBscFxgYGB4hHxsgGBsYGxghIR8hHikhIBwmHBseIjIiJiosLy8vHiA0OTQuOCkuLywBCgoKDg0OHBAQHC4mISYuMC4uLi8uLjAwLjYxMDAwLjA2Li42Li4wLC4wLi4uLjYuMC4uLi4uMC4uLi4uLi4uLv/AABEIAOcA2wMBIgACEQEDEQH/xAAbAAACAgMBAAAAAAAAAAAAAAAEBQMGAAIHAf/EAEIQAAIBAgQEBAQCCAMHBQEAAAECEQMhAAQSMQUiQVEGE2GBMnGRoUKxBxQjUmLB0fByguEVM0NTkqLxFmOjwtIk/8QAGgEAAwEBAQEAAAAAAAAAAAAAAgMEAQAFBv/EADERAAICAQMDAwIEBQUAAAAAAAECABEDEiExBEFREyJhMoFxkaHwFCNCscEFUtHh8f/aAAwDAQACEQMRAD8AQI2LR4P4XSrvNWslNFOzMA7f4Qdh6/T08p8CQgXP2/piKrwrSbN9v9cB6ZhCdh4elFECUdAUbBSP7J9cS1srTb4kVvmoP5jHGP1J/wB4Y1bLVo+I/IMccdXidplo8W5vhaSi5ShWq7HSihVP8TqLn0HvGOdlEkkKFvssgD5CTg5+H1B+H6EYFqZWoPwN9DgKa7nGbIV9cSBh0MntH88AVNS7gj2jEY4go3OCswajyi56wPkcMcvTJ6Yr2U4qkixjqf8ATv6Wx0HgGe4cAC71Gb+JIH0Un8zhZJmgRfl8i7WVWJ9ATiHN5Kou6EfMHHRqHHcoF5aiKOwBH2jAGf8AGeXSQoL/AGH3v9scQP8AdN+05JxPI1G/4mkdojCatwep0Kn3/wBMdB454l86R5dJR3CLq/6jJB9RGK954G2ORphqIctwavPRR3J/pfDnJ8KI+KqzegAA+8nEq5g/+cH5Oi7mACT2A/s4epBizciXJL6+98b+R2M+2H+U8M5h9qRHqxj874Lq+DczFtB9NX9Rhm0GjKwEI6D64zzCN/7+mJ+McLr0P96APk6kn/KGLfbCdquB1jtD0mHHNgY1bOHC9qx740L47UZ2mHPmj3wO2YGA61YDpgOvm43MYNbMw0I1fM2gWH0xAtbT8IE4UtmSdifcAfnhrwimI1Me9/72AwvMpUcbmTZMqgWvMLqa2GqtUYgC2prKOu5gDAn+0aPRh9RgfjWcYoxWwUEj1I2n+mK0ueqf8wfRv/xhaYdpy9Pe+Tmdjypt7YgzTc2CMqLDviHOrcfLGl9p6QXeD6sYWxgGPdOBGSFpkRfEVavGJmTA2ap2wQybzCsT8W8QOnKoERaR/rirp4grN8RQ/Omv9MN/EdDlRu+oH2j+uKZTqYbe8S0vHCM4r1aak031MAR5ek3JHy9d+uLfW4dTEQI+ROOR5bMsrAglSCCGEgj5EYvDV8xUdwuYZNGWpVbgEEmkhaZ2kkmb4FgIAfTtzLJ+qr3bEdfhX8f2wgXxBVPkkNpD0tTAU9XMGdSYjVB097YPzWdqs9KkjLrekKjPpMQTCwpi/ecB6Y8TfWU8TTMcNYHcHAz5Nx2xumergVkKI1Wgw1XgFSCwI9bbYgp8acikXohRV1FYebKuqdvaDjNAhalM3pI6kGJjvBHuDY/TFoyXjPNUhpCU49KYH2WBim5fxCj+VyEGoWESDp0xvtvgjI8WWsRFOooKyGZYUx2MnBhKnAqeDLhmP0hZiNkT1Cf/AKJGEeb8YV6u9ckdg1votsBVlBBB2O+FCUVUkKIEnAkCoYSG1OIMfXAGd4k6AHSDJi5PYnp8sF0kwPxnLAqsuqQ25EzY9O+AUqGF8Q/TJG3MGo8drNqK0acLEkAmPmZ9NsNMhQq1FV9DOxiQCFCggm9wPscJuH8OpMyp57kuQDoVVEmy2vaT87YtmXoIKBXTOlU0ht+YFRP3kY586qxI4ENsBXGLHuMB4mr0kSwSox5Qg1kgTPQ226dfTANLKeYT5jNIJktuI/uMAZ7jreYTL+UoCLqHQCxm3xXbfY7xgTNcRYJSYQdXmEg7G43w/p2LZB++0n6nFpxkbfaOqeQUEgkE2Nt4Or+/pietXEimu2mT9QB7b4X189l6akAsSyg2HTpvKgWiPngfw/XLlpvAH3LE/ecPzKGDP42E87p8J9UXD87TlCO8D7jGpo0l5YQx/GMFVALTtIn64qvHs35eYqoFWA3Ydb/zwnFkYJtPTZUv3TrmW4tQgA1FB9bfnjXPZ2nIiov/AFDCeqwwDXAx5P8AEEiqlvpDmWGnWVtiD8jOJDhL4bcK5wy49VDKcK/iCDVTigk8TjSrRtjneayNRqnLTY/IHFx8JZSpTpsHVlJaeYHsP6Yq1bXFGrqD5/IzYiRJP5Tij5/h6DOClHKY5Rb8JP8ALFgHh/OVHqFWZAHaNbusiTBURcY3yvhLMsxNSvoZTAPM5NpkGRAvHff3pGcAbxDAGM+DeGss1PmpKZ2N5+YMyPbDLNeGMvUILK0hVUQ52QBVG/YDCLL5LiSKEQooWwYtcgGxiSLj0wypUs+GQmtTKQNYYXB2aCAAR1Bt2PcqOQ3YMKsZG4m/GuH06VTLMH8ldRpE6woCLTqOBJIuWAG97YCfPUnCVf1gLUoBTWAqJVhXLxTRwsO5cLuSF1+mDquVrueeuDpcun7OmdMhhcMhGxid/XBJyqomp9VRjsqyJO8QJ/0HQRhGQZXYaL4815vt3EU2gWYuydJP1pqRqQazMKkujMyLTJ8wEAaFBlQGF9+mDH8NahQQF18oFQCEeda6ZJVtgIJJA3gTjSlk6a1kzFOkUdVKwtLfUAJYhdRaO5tg05t9QEMGiRyEGAdxImBMTirAwRKc2fMAg9pVqPhQU3VhWU6Sm6VFsqFWjliWYgxPQ9secF4S9BjPkEaYL02YkmQRM8v0AO2LNXFRgQUMEAG6CQJI6gwLx2vgPO1DTps7IxVFk86GBv8Avzjj1WM7A/qJqY9O9RZxrOrSUmJKoGYTvqkj7RhPw3PGsZCEST6/yw4p8dR1VgjkdJ0WHu+JKvGQBIpt6EsoHrsTg2axVRgJm2Vp97YYeXRO8tG3Kf5jCPIcfWpUakVKsvqCD74alybKBPSTA9zBt7YndK+qF6jXtCVemIADC2kEBbWIGxGIs/cRTjdZ1iZCzaJ3liZ+WEmZ4jWGoqiEBgpILG5iALCTcfUd8LqnHqskcimY+E2gkG+ruCNsGuDWnxzOZsikE94RX8LhlVTVNpk6Zn5XsB74mPhimUpoXchAQNr6jJm2IuKZypSoCt5ytqZQoCCCSTP4jsAcFLwbOy5bMKAA+kBjuh0kEhRBBgdr4LESBamDk1MaaeJ4XobkMZEXY/ywXleE0qUhFid7m8fM4l4ZwfQ3/wDRmCxnYsQPiqAfE3ZNUevoSCuJjKVcuU8xUB5pVkDQpI6ydwNgTcQDOCZnbYmKAriCtRHbEDBfT7YO8W59aWUNNWUllKqFI5VC6dh3mJ2MYm8N+B6NXK0ajFZZATy4AGhvOe7lcyGaZgoqOSSzajI+FZkWA6GdumJuCZl/JWppC12IgkA6ed1G4jZYwtWrqDKtMq5VxINuYMp+Vmx4M9UUQ9MmNNx1KENJIsSx1T3xtfG8Z25h9DOViWPmAiEGoqLM2sm0bQoHuMTPnq4qCmtWQXCTpWxkSNtwMJ+FZjUzpzBWYEELJBCqpsdxCkxbffEZCkaixibHbVzCSfUAtg9CBuJ39O8t2XzbvQJYkyXINvhDFQbR0WR88T5WpVFVT5rikr01YXt+JhGmSYBFp/KV6Z1UUKGGlaegXEnShRo9S0+5GJchxLyPOFYqOemafMpYrTRtTQDJI0n1l4tbB+oij6b2MS2NmGxrcS0+Ic9RVqamdyH8tiCshCs6f8Sm+wM4o65+sxLLUeC0pDNpEEtDarMulWETuLzh9nc2poCorBFemAqg7WMW3XlCzFrEbxhS6UWalSL8q06pEAGOZStpABVdS6ve+2EYdIGphKHHZeePxjjgDFHDVPMqkrJQlCBLQxUMxWIAF4iSbThlmM5SpvUNKkDJVOdFJXSur8NpIqLe9gfTFc4JT8qvUq0UZ1ny1J03bUGaRJBgiPzjqBxDNOppl3IqEu7ILAk1XXoYnSgsItGHZVBsr3gYWAYBhdRnWrq/E5gDRlqSkQBDVGNRrDrEYbrnP29O0xqMSB0jr88UvhOeNXP5uqSJLIJHXQGSf+2cWBQBUDkAgcoB7kT+ZX74Zixgg3FZWINivvxLV57EEhSBqiSd5DGN56E+3qJXZrKp5nmGl+0gCdMjrB3ibm+FOX1pUcltTinUdBMAtAVbHaWeBczJxL4bQ06QWpV1PVqSNX4iCC4XvKg+4Y7Yiy46UmVXvsNhCOKZxadUBnSDB0mNUTHcWMH+vZX4xzg/2dWZVKzpAmLy6yRBMggm+POOPTaq7sw0qogysGEncnbnn56cQeNUK5ahR/eq01jstNZb8sQp09ZMVcsR/wAw3eka+wgWYp5al5a09JUIurrzXBN+9rRAjpiKtqaTR+ECGCgRDwBt16E7mewwlqZldURe4kXPS0fMHDCrm2pUW0VFIYNq0zYgbTAvBG04+rdRwDdHg/E8fFq3YituR89pWspxTy6rVAuqWJ3jqfTFq8P8dau1QmnpWmmokGbsyoo2H7xPscUepR0hf4lDfUmPyxY/C1c06dULE1WRLg7JzWO34vtjyeo0lCxnqdLjLuFX91GHDK1Go2li4YCVOq2osSYCiTeNydunSPNZNxreCoVNK6gJhVgmL3sTO3MDj3MZN1qBqegGbR67zM6t9vaMMKwpEJSIEEft6iTbluBuRcQB695wGNwwLKRW32l2QFVCtzvVRRm4KZKi0xFSowPYk6Pbf2wbl+DUiikXhyzE9YtGAOJa69WtWpoT5PlUwqgk6W8y8b7qPrjzK56qiMmghjdQQTM9u+FZEf8Ap/dmLwtjFhpHmWV60GlPNAKgydot1vAxDqArLawaCIgyDcXxbfDLpRYNVK6hJJB6k2km1hb/AMYg8c5fLuwr0qiio3xJDc5HUN8OrpHXBaWC3F5H9/tFjuYFxbKMc3RQyRUKETtAkuv0B+uOw5fiq01CBRyiNh0xy7g+ZOYzGVmZoo7GBM6iq9J6Aj3xfaOYRRBJmSTY9ST/ADxBnfSRtZqIetR3AnI/1k2Uzp1Ei8XEKfs+/rhh4azBNCoal5Aid4liD/fb1wnzDMPVQYn92RJ2udsFUOImCCAJ0wR8/wClhttj1gN94tj7doS9WDpdFaV3AupBOwvMx6dMDmrQZAwfqbQ8jqOUA2grt/XEObzEBmEEAG/UlVUCbbD8/rgLIFFoVTpJfSAvz+EdbzMCO3qcE6gtdzkJ0x9m6Zq01cP5kA3G0ST2G2I34NWqQQF6dSO3t03xmRdqVBaZsRM+n/jb2w38LMuk+bXqguNQIAIpwTY6wbwVtAHrfBfyUQF7/GCA7EhSPw8xcOJVKSsjqsOxNirbbDlYxBix9cCfro1liACVI+GBfextfDH/ANP1WcwVJ0lmUrB3M3BaTqJuIwDnmUalUFQRsSTGk7SZO7C8jY97jjFAkTiwJq4fw7imlF25WaoD2ZtQJ+cOw98b8eo/tqOssFFOms2/CBrO1zJn3wly+RZy5BICBpB2aLWsTMn5WjDivlQ9Oizl3c04dvMPcraQdydrYGzq3MKvEV+FgFas97lSf/kP88O6PEWDPqjQ0lSR8MKVkerMVE9owu4LTRg4pFr6RzgdnjY3vOJK3BKp5V0Gw1ASDf5je3f3w5NW9QDp7zXiHE/Mby7qkATJ6s1wOlgn0+lmzFZRWphYAo0qzhVPwkLpHudcib2PvT63BswhlqFXTNio1CBETE9sMuHZg1DX1Eh2WJIO8mbWgbCP6YV1RAxrfbn7w8O7MfPH2ibN5t2FdFOptci4MQGCjbcrM94Hpiz+LKBnJUxLMBUNzuYRLn5vvhPlOBMpQ8pM8xLz9tNvlfE/ijMM9cBQxK0xAkndiW67Qq/TES5A2dNJ4s/pUfkUHGQe/MrzxrJJ/HHLe15/MRiTix0ZVR++CdxMlgDI3EgCO++JMtQHmKGtAJPzn1xHnqAeFuBq1CAPUxHa+PUPUabo8yf0xp0n4k/jrI+XWRVKlVRVUBpgBUI6CPiNvniLh1NQKdNmIhSWi8li2kbzMMmwxtxGmakGYP52A/ljKVMotypggzN7R6YkyOKAG+8t6YaW1XUZUShaEaoo2MA9idQuSLjqPSN8CZtEgL5kyJgj1t9b3xrrptDNT1cwidJ2HKJtAkbAe17D5mhpVng6oMd5i2MZ1HsHc9pS2RmGogcf3k/h7iSU1ZmcprqkzoBGkAAQSpuDOxH8i+4fVo5x6gDvawMwXkQSSP5HpcnYK+GcAHk0mLIWZNUFSSNRk/hO0/6YY8J8MmjqfzFDkzA+FQJthZ6lPcAd5NjxWRx8x7V8OU2VVJICmQBEHfcdrziSvkkJRAoIDCZ+R++wwPlOJzNP4ngxzRMESAYN4kx6HEuRJDatI0gElgZAYEWnqZnbs3bEzNHuKgnCqYp1s69MQF0009GO4H+ci2LU2Y02vbFK8M8TQUnL0a9TXWNUlVkTIYDcbEAxh3S8SUY/aJVDyZGja5gewgYk6voeoyNqXGT8+RQqecjrZ3nNs/mQVhQfhYf5iLfe2D/D2USHRhuikyO5aPuD9cLc6tiQeYRb/T2xLwniYUvqBPKBbcwLD0EDf164903W0EVxIcyYbTspDG0n0k+httiRMzDIrQUVtWkG3Tt9bjEtOQGqEHQf2cqI16QNUHpMiT64CzFAOSySAXIVNyAq6j84mJ+XrgiBQmCyT4jLNZtCoIkaySQTtLSRYbAGMWPgJBpkEarjSxJOoKNRAEbwrCfbaIrT8JJpgA6iCSCBG8TY9ZGJ6dWrTAK6WVJLaTqjUI5gLixIk2vhGfC2RQRxG48gUFTLfk875Wp6syyrsf3ixFoMCINh22wiyOS82s7svmpSqBCvRmY01vvyjS5PyEwLjXK+IeVlYSWSA+0LCqBAFxpA+VsGeA+IOiVYhEKl6rkcolyam8SdA02J39sFiLoCe5IH2EWVRmHwCT94V/sJMxmSVAp8o5GkAEySoIk2UAmxnWOgwBW4cqFqXmwE+ECoWAvIgtErI+X5AzIfrDq9U1jTo1Eqs1Gm2mC3lmmWjcaYT0VLWYjGVBTbN6PLBXWAXv8ABl01uTaAGKuDeZE41c2olRW211KGwKvvo0b2sxf4dyxWoSSOapt/h1g+2qR7YtwqIh1tAEQfbCI5RKDIik6w0uCRYsimw6CSfviDirkqZMW37ACSfYAn2xZ077k/MhyAbS78G4tl6p/Z1kJHSYP0N8VLxjVC5nMtpVjyHmEj/d0+ntgSpwJPIpnS1NiELISJIcEgkER0IuCQZ7YB4lwyoYp62LIq6yCLFiDBWdlBCxET2g47LkXY/MPHiLWBB+IcXVNAXQfMJAamai6Yj8GrSd4jT19MQPSrtzkHVvOtQIW25AEie+M4D4dfMvrkfsQGgqbyZWdNxsTMGww8q5KsCuqiISdRpl3BJINwx1g6egT6TOJm0arCi/iMRSBpJ/OJGOYSJLD/ABAkbx8UFTcRM4iYnUCRYzEEG432P2xbsrnKSl/2nPHwl1+EKANdJ01Kxtv3OK1m6AdfJUKcwzIENKPxVEW8HciTtsfTAFQTVzfp/SQVao0z2xCgDiBfpbFgyvAkCrUZalNi9NQjAHWXdUWzjVBJMkdrxIwHU4IH0ssEyC6mw0zJIa95tHoIOB9LawYYfyItThzr2Ikdf9Afpj3xHw6pRRQ7g6ybAkkaYkGR6jYnDKrkQWXyxURGZx8ZYDS4Rfi73OGHHvCWplFTPqIOlPNULdjYSDcn5YbjwMxuuIGTMBQiXK8ZTSoamZAAkML6YjdJ6d8eZ3izadI+s4G4vwKrlHVGek+tdSleYESV3IF5BwOp/eQWMWLbj3ifbE56VUN1Gpn2oRtwBlNXVU26ahuREjD/AMTcSPkuRUGhU2tM2gCAIHS2KfSzAFwGB+YI/IWxLm8yrhFYwC6hiegmT87DAHHbiGX9plvyyJRRUAVoQKQSwAMKzRoYbvXA9h2xtS4hRIuhFz/x6/c/xYHTiGUqHnJJDsQUqKAQSNNiwJ+FTtvj2pwvLMZBzAsOgOwAxp13LsTYtAU9vmUbNZcoYidRH0/v+eCuGZZW1jppkd5mfsI+uCKtDzF1NKkg6JIC7gAnrvI+kYCyWaKB5HNpCj0n/Qe0dsV8TxQdps3ECqim4BRTKqepBkT82AnvGJuDBWryg0ruQb6YgkSSSYJAk+ptiWrlzUTzAVhTEbHTaCB1BPX1G8HAhoVcqtOtIZHAgqbqYmD2OmGttIwDGwQOYxfabjxGLGp2NRgp6QsKfbWGww4rk6CgPSlHRXZXBJANIqF1R+E/wiZMXxX+GcQIpBmM8zKDE9mYx1uxOGHiHLCMusa2syaYjSQDcnadBvOMLkFV7QNNgv3ifP1TqZmUDzGJDJemQ1oBEwZGxg72G2PM2StBVAhZ6sIII29dRXVh34d4etPNGnqLCaYdf3h5lUEGDtCjru3yx74g4NS0a6I0hbvJYFdRGwblNwZ5u18DpJN9hGIwAIOxkLcYdi6mDTIRZ0gGTzbxMCT6GMSVOLDTWJkKX0Km5VG5XHqYAJB7EDfCHQiNUWpqDgyvx9SLwRK2k3F4xvUVWc+U3mKo1QeU7GZB67ztjlwBWsfEI52INy410YvTqmNFWWQ31EDq0gXMj6YKoUKktVpIrmnACsYBm7+4ST9cJ6meUpSZCeRLggiCAvQi47bjD7hGYhaNaQaas2tBeWqMKbMd9lkaRYwDG+Grm0CKKeo25geVZWevmKpBPK7DpcaFQT0ICj3O04Bai/6zUqEgLUVjVfVyi8sYDAxMiATf3xLna6pTp00YF6j+bUAWxJbTEdBqLGP/AG0+eFlXMctwysx5QosTAAIG8+szPacLyFmYHVwNx+MuwIgUkCrO1+BtLXkuDVEylRk1LUqV9UKCSAvKgkREQGk2BtI3EHBuHZjzaZrF9LuzSrsVOiZZ2ErBIA5o1AiDuAvz/GatICii2UKjtc8tE1C5Xa5Y6w3tGD+MeI2pZGsCV1mgukqf+exSmRYCdIZ5gbCwjAAHVUnZjRqKOBVqNV81mqokZiqwpAhY0U7LZvmB0+A9sMK3g3J1lNRUVRMSraPYCSpvafngHj9ZMll8pkhSV63lqzzMLJJbYgsS5extAMi+CsvxA1EGmnyNSYg7BIkTBmSX9Z+2FZnZDYPPEpw4kyJ+HMS8VyNTI5jKqK9TSaitoeLBCom1jZmFxNjg7KJmvKpO1GpUps1El6dNW5Vq66jDQxcDSFXTovBM9654u4sa2ck/8JVT3QEt76y30xZRmc1SzBy+Xd2KU1BQGRyIoaFa09wvWcWB6QSRcWtiLqvyglPiCs1JSyBhOoNy1ATVJA0m91AJxNxXNBc0NZgKGZiRNjAEjqJIt1wXW40xAXM0hUCkakqDcEiLVUZpmbgr0jAHFkyJy1avl6VahUpKrKJ5OdwosSyxqJsI+FsGMvtKjvMOAqwdtwIPxnJFg9RNK8x1GmYgjeV9ptHfCk5lYWVIDAGQfY2jqQfqO2IqWZdlaoy6nqoQNPQCFJI6mwgD5mDEl0+KUVpBG1q4ohYdLa1FiIkxPcDfGdOhRirmx2JhZsyugBG/x+kFFZF1sCWEQeXYTbrBNx9MQ068idB0zc6TETfb6Y9zyp5XK6NtJEA7j8MCBvftGHHB881GiiVEkNJEtEh9gAYQmCxGo6jNrbOKIxseJPVf+xQUpMYUx6TH9Dhxw7wv5tMVFqWJYDr8LFf3vTCriue111ZQVIiCCJlRJMr/AB6j3uJvjq/hXPBMpRDk6iuo/wCclx9mxhxEcGZrqc84bWLSXgMi8pcGABfb0BJFupvEgnDhgr0iQCtlid5A3nrM+0x0xWf112q8iElLsRvYzLHuNhHQAYttDjAakqkhWN2gQEEwBHRQsAeg64Qi0d+JzGxQldTNCnqUzqVSF2s5Uqp+SltXt8saZh2fRSQmBGjf/iBdRI+YBP8Ai9Lx8XpBq+mkrayzcsSYG+odCSNun5w5XOPsh0vsT2tECfn9hjCBRIjlJDCWXhHA0rUG0AoNRaJ+Ejl33g6ZgzvucKqtZ6dSmrE6AwYGDcQVMSOxbad8WbwlL0q2mAGfSI2ULTReu4UC59CcG+KeHJmUHljywop6QF1MFViqkcwAIWCd5Bi8AjdtAsbxVkMx7RHwjMq2daorAR5YBgxZajsSNV9gxg/nhvS40Ghqiq6u1SP3oHwqZ5WOmBuAfc4pfCa/l1BULgLrKh/XSdJi8BltudjPqwrgVKdNDUFKr8QYgaW1RbUNiCu43IOAC0aM07wvM1Eq5irWHOp0UlAQydIBc6bExqUAC8sN74M/9M0horLyMBq0uNSfCehi9wBpY9LYrOXoVKILAHzxW0HYsdQRlHqZUd/i6HFr4jmg2dorTchDTXkF1KzWkEbGNMXxxGk6gZar6sYxtwP8wbL0NVbySoQpCnSSZ5FfVJAaYYbiRAF4kuW4DVCaVa9iV2B3jsDttb54WeHnU5+pAAVazqANgEpooHythn4s49UQAUmCMWVA0AwWMCxtaZw0Y0dDrkZZlallI4vTc1mFQMjzGhh+EWHXaOokeuGvAa81113FMmoxnohlAJgfGVt2th3kOM0qyeVnEWspJh1XmAmA0CDcX1JBuBBOEucp08pVqBGc06mpVkwyqC0EExO/WOl8LbErC13A/SPGUj2kEE7fBgXlmrmDSB1M9Ty0iRaLyJmJAJB2AInFl4rkxUz2UyYFjUWtVG8JQpqtNT0gaaie87nCbwzlWSv5iEPpBkTpYTa6mGU9jt64d+EM75ubzOebm/4VOT+AQd4iYC77yb7k4WAsxbXxEHinPLVz5dhLIhpusGA9N3BidxEGfU4LqcS05VF5uZmc2A5KZ8xiL9YCdJJxPwfgycRzGazBHlh2BoAtBJ/FPzWCYBgvaYup4/wyvl8rUq5q1aqy0KSAg6UU6nYR0OkKPRiTvhD4NWQX2qWJ1Srg0gb3EHhnL+dm6INy9UT8iZb7ScdVpJlqL1uJOagBLIFgHdgrEAXliCd9ifbmXhWqKNfzv+VTqMv+IroH01T7YunEq1fMZFFGXil5ukLBNQqLaiTYEy5LREwdjisrZki8c8y8ZtRUUEAOjAGGAKsDcWIJvIvbFB/STl6WXygWkiUzXrLr0zBFJXO0wIZhtjo2Qro9NTT+CIH+Xlj5giPbHL/0yZjVmMvRH4UZz/naPyp44RYuVThmYAQN+4bj0eAfoyr9ThvTzCkDbSeh2+hlcV/h5OsoR8YKj5kcv/cBgfIMRUtMztMX/LGtNEtR4bQe7IF7FZH5WwGOHaXinWdWWYkg72MQVIPSwxqM21OQ0gnbVy3+YEH2wKnEnVwKkMs7kCRPqIxwJE4r4jDNZFqelwwrMUqLULhiEMwCDMggGQSTfcbDBo8VVAFXyF5VVRpdgIRQot8hi2fo4GoV6ndwN7fCJj7HFoqcKoEkmjTJO/7Nf6Yx8j3tG4zgArIpv4M49w+si0/KoqdTHmbpBIF+9phflvEHTP1HpVdSz8QZQO4uO+xv6Yh4Q4Vyx2i3zNsMf1U5mqtNfXU3RIEyTIgf2J2wQA02ZKSdU04KyUuUNrq141VbyosSunoSwu07CfQr+I8PZXPlBtI+FysagvxG5vBkT1i+5wRw/NGg+nSGvIZmIS8qHNuZIOwsbG4sZczxk8y1QFBLEaR0mWPW5aTPUk+yMjMN1FyjGQRRjfgNVloIlMgl7kEgSrNpc3EwEmQINxvcMdm+I1UBNEBl0oYYAHTpqKSWAnVqK/DI26XxB/sYvRTdW09LRqWGFvQxhJxGu1NadJp0gnVHUR03t8JI7r9aWxuNLHj/AKiEdGtTNOIZCk0ssEaoA2NiQwidgQBPWRHWFR0g6QpIBuCZMTIvAm3phxwSut6RB8ss8G/LIteDuV69SB85OF5RfOzNTSSq1DTAWbaiFZh/hQETNtYOBtFx/InUzP8AEW5Qxpqo91IMTGwsfYHDJs7QqwfNek6lzI3YadMIYgGDYmNmmLHBWc8GmC9AnSJjcggkgKexEHb95bXMVfM5MoxWbjcQf7I9RY4UtOLuVNkqlrjmWbwG5Z9bGWapVZj3JAnDjiCB8yCQxSkrPCLqOsqRTEdb6j7DCPwLylSbCX39VX+ZxYjkkVGzTO3M+qxsEpyII25oI/xMNsZmyBMR+TUDAobJvwN4LkuDvSNFqmyc7QDBFIFmCuDduXSQes3Ow18V8N01F181VUTWwJknSNUgH4dh6ARMYJ8PZmpVqBUZmoO4dlJjmV/NcexVQV2mrGo7438ScaUkjMh6bK7mnK/CdA8tSYspEsW2JmA2kkSrqUe3mPfJrazKxUydKhXp+aXVSzSQ8qwIgQyAMpWVk3sbTfUy4fVNCm60F1UNbKhJAqEtqIgSFcwJgR0EkxiTxLlASE5f2aimBF2Zh5rf9j0h6R9KzRq1KMhQCL8jzaYJK+th9MejjwHJjDHnx48SJ8gV+DXY9jLd4VzKAvTp1AUhTpO4YDSxKHYGAfnscJ/HmfNfMpSJlaK2EzDPBbfpAS3SMCZvMU8wB5R8uuoAWnUYDb9yoABNyADBvjF4DmGJdQWqEkspYawAQqsZI+NtWkXJCT1GE+npfUTDBsVLB+jPh1MvVesqkDQKZdZAYEkmSIB+HFg8QwtRGDOrEOQwPLYtU5gRcFZ67DbCLwlmvLVkMq8nUpEMDsNSm49xg/xTmiuXcJIlSCBtBsbdDB3GGYm99TH23jPwDm6r03SoECrpZIBBHmanZWvcixkdSe2OcfpDzJqcTq9qYVB6Qon/ALmbF5/R/ngtJ0qTIYMx3KyNPN12QGb9dscwzdXzcxmKpnnqMwnszM35EY0imInXZuBl76hZ1II7TuMNa1CkWIhTeRG8G49bTHtgPyQRfGZmlJWNwv5G2MmiNGyhKQrH/MSR/fyGA83l3QToEx8SiwPyxFl8zVQRuJ63/wBcGVs2HWCQvWZt72tgN4ZIqdH/AEdMEyVMlYas7kbXKyvWNwkx2xafP/gf6A/kcVfhVEqlKmLFKFPUwjULM9QA92OkdLB4INxL/tPJrapWKuNx51c/I3fqIPvjoucjyxkEYeZM0zSD1W0imIpqPxsSdx1JEgjtJMzAr1B4OC6uYZdvxCPl3HyNj7DsMawMFYy8RcQSqtJ1jzQAGAB3gTY9JkSdztscKsurVqlOmLyw1E7xMnG9DKMSJB0kwWkSTGo732gn90fdtwzKolfVSayIpljI8xrEGYsDYkx7YwaQahMTVidKy6agFUAAbk7ADrhZ424TllpKYJJEve+mT+0kWt0Gxuu0ENKfFEFNYlWUxWAuZJgKANw14Y2AkkWaBsk6PVbMkSpOmkRDAlQ3mqBIGhQNMzBLDqCS1sxbccePMFMS6fnz4nPf1WpS0iQyqJQhrMrkHUCJsRYx2xYvDVFf2NMHnOusz2jVUKsTvJKIoBB3IIwVxzw0z0KWYootIsut6ak6VDAFmCLy2nSQoHQyYINRyedq0g6gfCCTNwosCR6GYJ9emJMpLgBfO8rwaBeo7gGp0HNVpq0KSOVHmU2qr35gNDnqVogLF5Mzhf4g4SlaYULMlL77aY7GD13+2AsxXppRpujBq4pwx1DeqpLCIsf96RczpebnG+c40BRrE2ZQw2EM7+WAR1lF0jpud8FjJL1XMjzKasHiV3hzEUqmkyR5mk7TAUziHJ5+quWWmhLHzGJUSSACDAvYEmbdYPTDbw/kzrCFXUHWQHUglYAUwQNwMR52kuVYkPpnoATI6ggAkC2+KcnTlkNUaPebjzFG+Y/GZrZemudRKZROWqnWajI40GOwRZud5G8PMnxHLZwTGpUuwYAPSZZlp3A0ArqWRYT1xWOE8RUmiWIKBhVYE8rVJJEmIEG4723gRPxPhOXq5StmgzJXqVXJ5jtWaHVhMAAFyYi0zIxABbaa+JYChSzyO4nmUoUsxSDtU5mBqS3LpNS7LMabSF07cvSJwt4jl6aUwliyli5CxpEeswIG3zM4F4fmTSKorTAkAGYl3UgwZBgAgEdbyImTjvFlOWekL1XCrTUCTdtLqYFyACI9dpGPTx5wtGt+NpJkwuF06tuaPmU/h1Najv5kAEGBMSxMgA7A/O2LNwviFbLhkqg1aS6eUka0/EDG+nbYkCNsJ18O1PKLyscpHNHKQZZp2mBA3P0w/wCGZZKlJaUtTqlDKvMMZGkpHMDJiF1XX4GxJkye7mXYsOrHutV3g1TO0swz1LLV1KWfW0MzBmJViAysSDykAABR0GNMxnMyrCnVVogkMRGpU5yQ3wtyKfrgTidA0aopkQZpsZAkxriSDDdTNje4kQA+FZ+pQ/Z6tVM6gaTzpOpSpMfhMHcX232w/GNQupHkGlqBlqo5tEoV6tOpz+WZXZgSSFkbxcX2xVuHoNA7En+/th3xbOUWy4BoAFmULVJDAbCFIvAUbHqDbCluSLgSARBBmY7bH0x2ihcwPqO88ekOlsaspA+WDMtRD3BE+n9/lPyxrVpFf6/3+WMhAQXElLKiqy0yPjZVt/EQBj2onp7jDPwnQ1ZujJGkNqJNo0gsPuAMCRNnSOLqAlXlk+XqVREnyw0i4IAIYCekk4qfEcw9OoVZUZiFZjqA5nUO0AmygsQPQDF44plvMQjrBg9bgggXFypIna9wRIPFfFBWrmq1QkXaP+kBR9hjgmqAH0xTg3LvqEHp/LAWN6DwcawsRYjylXWoSoCKYMO5gKBcqoMAcxkkX+KJ3BWRphqbELpVyYB/d2H9ffCOsDII2P5/0IxdOG5IvCrvHsI3JPQDqcdiUA2ZzknYSsZvPVg13aQoSZiVtY99hJPYe1x8HUfOp1DVINMKj+XSblRQVYJAN6hKJq1TAEfiMJPEeQoLSZi/OrABgCdVhy9hvI/wmTDCJPBviJqAKLBD2QdntBY+v0BAboccRX0xlFdjL5ns7VgCqwQaWeqZACh5WlT7xdhMfv3kA4ofHaJydWm9Nh+01cjT1MkEQBoYQYGxYRYg4uOZylXRUqPVXQZNVyqkAhRJI1TAXZe0C/WhZzVn6vn1mNOjamhKzoRIBJA+eonue0YVhxszEf0/ve5uUps17n9L4FR7wfOUquYJNL9mqjzEIE66lifXQiwL/jMHBWb8PU1zFEIwag7NWgmfhOogk3KmUF/3cJE4e1Oq1OjUFapSBvIOtAfhIG/KQO8gxaJEzPGfOqBkJQBDAMkq0ANA73YR1t8xz42xtY4I2mJ7jRlu4xVP62L3WlpJ9v5zhX+pFmaoQxCCWKiSJ9PSJtjzJZo1anmNMlAYJmJ6T6bR0iMMKfEUp0A9MkVa1RqYI6KOYtE2soEzsepgYfjtcNTtOrJdbStZ8lFY010nSWYEcjROtkIteCOoJU7G53o8QFemiJJ0hpB3BY2uOgGoT/EOuGXiHyHojMUho/WmcAAQQlN9Ttp31hkRWAMGTHc0jL5g0nLLBvFtjB/CYsf7IIthaYWdNZ5EdmKB/ZwaloFCCbSWZZgc3LqgDoLtMddI2s2E+d00M3QY6agBFRuzAMRBnrY74P4XxJKwKmFq7wTvFzGK/wARreZVqVAN7Aegtb57/PGqd6Ii3IPH4xtmc5UekHUcmhFqEtJlJRZFrlQpmMPcjwlzQDZiNEjUp+JEMgNINgd+wF5iRit0k8rLKzFNTmVSASRO7XsLREdv4onzfF6wMzZ6ZVyGlSG1csdIBNu5xJlBLHTPTwOwxgQfNlqmdZXq+YwqEGpeDpB9DA6QBA6Wx4abJGu+mYkdiQCrCzLJHyM4F4Lka9XzKtFS3lkFo35p2HX4TYXxf/C3BqNYVPMTzRVgBRYhlGpmB1AKRqWZ6W9D6SELgbffYTyXJfLt3uUnL13phipOmL2lTJAhlIIPTe46RgPMZ8sNLhRezDoNojoPQYtviHwjXo0yaQapTJ5ltrUCbED4rjde20XxTOIZUqlNj/xJgegi/wB/scKxD2WYTGmoS0VlRcsNJWRp0m34mAF94vfAwzJWPMsGWQZFxf8AODAO+BqHBdaBiYYLJPt1/qRHrjfyVFPy6qwwutRVlbx8SC/SJE26Yoy4yRZERiyLxcKKK1x9uvtt9Pphr4RoaaxaAYUj6ke42xWcplXTqZaSGXnVyNgCLbbzBEXjBOT4+1NhB7AiLEz06j5+u2JMikDaVBhOnvxJaaFy2gKJvdf7Ppiv8B4L5lBKjIdT6nPOR8bM23viLh/HVflbkY/hbY9LdD9j6Yaa0/cHswwgZSu0wqDOQzjw4zHmK4iH5Vwywf7jFn8OcbShrerUhXJDreVi40gbkyd7fnimUakHBmcy+qSN/wC/5flhZENTW824/wAbbNVJjRTW1NJmB3J/E56scHcK4RWFI5kCKcHrzFdnYD9wAwe4Ji0nAvBOEq81Kury06KJZzEhRaI/vuRbuH5uMuUqc9NgSqiZG2nYbG4LEDV8IFxC8mQVpEcuMncxVmeJVc0iZM1ESjSg1GJgsBsD0OlT9iTc4sKUMvl8lUKgrSIUEmC1V2B0SCILAftgoJsVYgAWqtanSWBqmjVBK1FAEAgyPQ6pBU94PoozvEalVgg2DMUAsOdpMSZkndiSbKCYUYFUJ2ugO3maGCrxZ8+JNXkVBVWVggAA6iq/DF7Naxmxm9jGN+MZZxU89HL0qzWeykN2YA8rD773wyFACkSDLFIaYIcm4CRzLCj4jOxO0DCfOV3/ANwrRqCq4Uyu4I99RNx3ImMN1kmovQQtywUqpo0J3IVU9yu/sb4r9XNuNDqxDKvlrHY69r7833B3xbXpt5ZKqGhjKnZhBUg+hGAOD5VaeZXMaS1ClNQhwDGkXU33EagSBMC+GbgAnidjyKFK9zNfFuXZQKSxoydKmjyZmrU56xE3J1uJ7QNrYVZzL+WGp6VBAuZN5iN7SJMbGN9sRcWrmo7NqM1JqVBNtTEkx3uSMa8NRsxXWkxJ8xlDnrpX4vmQoJ+YxUNSACKDAg3H1Dwsf1am55WqDzA1/wAV0Hpyx636zGK9nssychXSR9/Uf3/PHZ+F5xcz5ysoVU0whF6YbUqKwFtk1TJid8Unx9RpUqTaWDutXQR+JDGoyN799jII2xLqIOloVA7rE/g3hVKvULV5NNIlQYLE+vYdrT37uv0oZajTpUalGFFTUCo6lOvcEayD7dsA0eGVMsgYSxZB5q9QepA6j03+eFHi/iHn1EAMqEEfM3Jn5QPbCNFtvKfVNX8VNfD/ABF6IRablDr1OZiZ0hR6xB+uOucO4zQasypHmqYI5QKhYcxW9mJ02aJ0e+OHU6pVwwMEEQexGx+eLORTzEsGKZgmSw/EzyzWEe5A7b4auJSxLGhENkKgUJ0uhxENmKtJmCVNXKjA6XUqsRMKx1EiAZsYxzTxzmP1rigphdOnRTIA67vaBeWI9sW4UJVqTV1zdKmLujqMzQABBm8VEEkwb22MDFP/AEcUWzHEGqsejsxN5LzIv3k4FNI9ywmLNsY+ynDzY9ZswNthsYjqRuLjfuPmMvuCPkenQz226iDfri857w8p56PxKCAh+A8ogbbbW2+mEWYyJp6ldW2li03knbqWAAFibT1jHsY+oTKJ5D4WQymcRyIAJRiur4tJsfmDv8mHucJqpZKqNWsFYXUDpta3bcdsXHNZbQ5BVgOhP1sRY+2Kl4kINVEttJ7X/wBB98I6nCApMo6fKSdMOzLaCorI/Nu3TYbNJBG87Gwn0c5Ph9RkVqdQlCJWHb6bdNvbCDOcJZqaOWMlbkkm26/ngUZiuAAApAAAu2wEDr2x4h0P9JqeoceQdoux4cZjDi6Rzw4ZZWrqwtxJlqkHAsLE0R1k+IOrKs2A0MBblkXn7yfXbcOeL5fSqK5jXLqxYhUAKy5iDIBGmfyjFcrkgBlMdCf54Z8KrnWK9QkqgIphxIbcCepY7jtAPbEzIBvLMLM3tnmYyVbMV3pAOSC7BW5QtgXYiAFkXjoCO5OFPDsuC8diCbA8ogkx8uh3wf8A7cr0HdxUBaqmlwbxaBE7BQFAmZ0gGRhfQy1QU1zCMbG7baWnaTuSIPuZ9XIrMvtP4QepUq9EV5Ed8eFKnSp1KVQhoEoZvqG4bfYAMDbfadOFfBsvqcNMwdTn5XHyHSMBLqzFVVLKgZok2RAbs3y6nDrgg+JEvTUlVaCDUJYAGDtyzbpPzwSXXuNmIyNf0ipfuDZL9is9RJ98JuM8KJDKhK6hFuomYPpP93OLU7rTUCbAAfQYp/GuJLWdqS1PLjbcajOxI2HX+zj1GZMeKn4AkSKzvY2lTrZQnXqGl1MEd4xZf0YZIl6tbTzLppoSPxVSJv8AwqD/ANQxpnso9TTTcacyF/Zv/wA0D8LdBVAuP3h23DLwTm/KphRMFz5i9QZgm8HUqgD2xC7+0EHY8SxaJo8jYyw8OzNLLfrTVq9Om1ZtSBnUOyhIQgbkFtUEeuOdZ/OLVzprMNQB1GBN0HJqk3BqFZ9Jxt4vNTOZzMVKKF6VIKgKiAFQaRv3IYgC+IvCfD6lVqmhgihDrqtfy1W7t0MxPuAJE4TkJY6u8fhpE0ng950SrwRzTp1XvV08zC2oSdMgADaDtYzETin8W4ItTW6poqr8QOzb3B2k9/rBmLhwPxIXrpQCa8vUAWg4iU8umJR9rwhbrvIJUiK54u4wPKzekiJSnSI25zVVr+q0yZ9R0IxzKVIBix7gTKI4G+46EdZw3yNLRobqro95kBZIFrxri89tpwtyw0oB/DP/AMkfkcFNWaBMxsT6SDH5fQY7LYXabiUM1GRcazOmtUamQAV0SvVSmhge5I39b4vf6LuHomWes4ILk3MiEAN/+pSMc6zkMQqzzG3r0E/OTi6cU41mMmaVHL1AyJSXUhQEWkENYMNUSZM9owsfQB+9oxhTkidPyfFKbEIDe8diF0XB2jnX79secbp+YqouiSw5mXUFC8xMSP3YEHcg7A4piValVRmqdPQgSCAfgZdIaR+6Vghh0FwOpNPitWrTdLazdQANSgX1aerTYCPiIG046yosQxiViBA8sf1nMVaIH7Sk2plJksgLXVt2GpwSpjTMCYvzWqnn5oiCA1QL8hMfYDHQ/DCfq2Wz2feoj1groIJ5SCQJmPjfRAjZR6gUjwZQ1Vwei3PvYfacMy9U/onV2H6xCdMozUveW/imVLTeCNMdkBvAHVhTVm9sD0eGqyqyaNLKCNTQbgG9jfBfHgVKzqUgzuVILqRMi4ABHtO+FWU4oyrpMSGYHVvZm3gxPyx5XSIHx7z0MpYHaUucZjzGY9ieRPceHGY9x06MsjU1CDjbNZhoRBJgnSg7mLwO8/WcAZSpDYZ1SRpqL8S4SyAtvH4srY9xIa/B6odvMKgKqu7gggK+xixJm0ATY9L4HSo7s1Kj8DkcvTkvqMk6YuSegnpOB6rsxJkktY9zsb/T7emLp4RyFOioaoZ8/TTUKoLK+osCCJbRpWTtMgx8JLnf0125mC3Nn85W+LcPSkyqlUVBpGpxtqiSB6DbDrwt+Bj+8SAOyWA+pbBvGuEU0D1a7eWBSnTEFnLAKqjrPcdAZi5wArGjSBFimge8Fm+5IwnG+qjByLRIjrjPFYgEwWkL16TJ9Bifh/BkVaTgli1MVQYPPr3IN7ggiIkESQVkih53Pu9RmMgkaQOwO49+vecW7hdR6VGmKzAJussQAQ5cLI9SWFQXQkgyrBSzrGDrVwunwagV8+JNx/OIUCR6UnB+J0IkKBJAWQQ+1m6RKSrxN9XmABasHzegeBZwNpjf19Iwd5DV3auoYUrrQUqBpSewkCT1679YAvE8hrBZRcbgdDF4/p69RirBgPogNJ2Co/t4i7JZ7Rl6yC2tVBBJubifqdj6YuX6Gs1FXMUf/bRx35WKtff8a/TFH4aaS1V88FkBuAdwPlvB3Hb6YtnhTiIoVKvE6tPRSYeVTpoACQSsQLC2gCZAPNtAGJWGliDKC+pQPEdca4IMqalfzfKWszI1NbBtbbqAf3NbRuABsS2OW8TzOs6EnROsrNtW0x0tYemLD4l8StnsyKgRkVKbKqapj4izbAAm0/4Rc4q2WEyep/ljqJaz4mlhVfMNomaf+X/7Y3FJiARsP5xP8vtiMWU/L/7Yt3CMkn6qklTUqOQFJAklhMA7wCCQPlh2NlB90mzMRQXmVbIU1FZGewUgkfLt79MP04ipcOGN1En5DYjqPTAnGODtTkkWn6H64W5fNNSbpbadvfCs2HWNWP8AKUdPn0mmnbPDNVdGkQCTNtifxR9Nt9/njTjfAPMpv5DGjUJ1StgSFZR3je5A79cVDwlxsvShv94lmH737p/174s3AuMMWKvLdyNx813m+++2++IbokGPF3qWcw8VpUyqHK6WQOQW7OFgrpi2kGPe1ryx8A8MkqP33AP+Eb//AGxH+lHiArZ5KanUtJF221PzmPmCg9sP8tw/yUSDBAUE+v8A564V1+UJjC+THdKNWQsewjqnQFbzKrUyzFmYKBzRSDGF6glnRfaMKst4LSuoqoFCvcBgQe19LqL72A+QxNnc/UNJlYm8c03ENrN+smL+gwZVr5iwyz5XyQqhNZGqAoF5vMg74nwZFK7Ss427GpxfHmMxmPdnhTMe4zGYyZPDhvkKsiDjMZgH4miF8G4UGaqWMKoEnqAwaCPpt/ZHyGinUUlm0FSx5mEBiwfa5JRAPmR2nGYzE2olm+0pUbfnDOFZlqjpVaXpUpWiKkMQeZ5Nxe294gATAxNxKjqo++r6yP5nGYzFKjeIbtBeHwz0qryNLKWYR0NmA7ze/UdQYw+8S0aL10y1KRTSn5tYwBoRRqKpbcrHfde0DMZhLH+cF7b/AOJiORdQ/hXGHqUartSppTWkDRVRtBUIpggmx69vbCKnWZ0FaRLFp0iBb0+uMxmPQ6Vycmkws6AKIpq8KZ6X6ySAHZlpL3FONTHtcxBvvj3IZhqpo5eo0UvOB0mTF4In3I95xmMxM7EkzB9Msvj7LUqFAeVTpo9VtEqgB0heYSOh5RB+18URFiBjMZjsW6bzmjHh1HUrOOYJOpdrQxkHuIOLBwqrTNbQl0VAqz0Z2ZhYg3LGn6eojGYzEb+52v8AfEsxIuzd9/7R34uK05p01GqTDGSBN+UHb/zvvjnWdy1SYJkkwNuvvjMZi1XKUo4nnsTqh3hmrVR6mkgeXTd2BvPl3I+9v/OLxwXjFOsNYBVwBq9N4v1G+MxmE9YihA3eOxOdZWUbh1bz835rXmoXv89QFumwx06m4qqReRY9wTceh/uce4zHif6v9Q+B/mWYPp+8E/2c46jT1Hp6dj9vlgJuF4zGY8tczS7G5n//2Q==)


The DVD rental database represents the business processes of a DVD rental store. The DVD rental database has many objects, including: 



## DVD Rental ER Model

![App Screenshot](https://www.postgresqltutorial.com/wp-content/uploads/2018/03/dvd-rental-sample-database-diagram.png)


## DVD rental database tables

There are 15 tables in the DVD Rental database:

- actor – stores actors data including first name and last name.
- film – stores film data such as title, release year, length, rating, etc.
- film_actor – stores the relationships between films and actors.
- category – stores film’s categories data.
- film_category- stores the relationships between films and categories.
- store – contains the store data including manager staff and address.
- inventory – stores inventory data.
- rental – stores rental data.
- payment – stores customer’s payments.
- staff – stores staff data.
- customer – stores customer data.
- address – stores address data for staff and customers
- city – stores city names.
- country – stores country names.
## To know about customers
Query 1: What countries are the customers coming from? 

Key feature to show is Distinct. Inner join will also be used to return Country.


```
SELECT DISTINCT(country) AS "Country", COUNT (country) AS "Customer Amount"  
FROM country
JOIN city on city.country_id=country.country_id
JOIN address on address.city_id=city.city_id
JOIN customer on customer.address_id=address.address_id
GROUP BY DISTINCT(country)
ORDER BY Country asc;
```

Query 2: What countries own the highest sales revenue?  

Key feature to show is Order by. 
Inner join will also be used to return Country and Sales Revenue.

```
SELECT DISTINCT(country) AS "Country", SUM (amount) AS "Sales Revenue"  
FROM country
JOIN city on city.country_id=country.country_id
JOIN address on address.city_id=city.city_id
JOIN customer on customer.address_id=address.address_id
JOIN payment on payment.customer_id=customer.customer_id
GROUP BY DISTINCT(country)
ORDER BY "Sales Revenue" desc
```

Query 3: What countries have the largest customer base? 

Key feature to show is Group by. Inner join will also be used to return Country and Customer Amount.

```
SELECT DISTINCT(country) AS "Country", COUNT (country) AS "Customer Amount"  
FROM country
JOIN city on city.country_id=country.country_id
JOIN address on address.city_id=city.city_id
JOIN customer on customer.address_id=address.address_id
GROUP BY DISTINCT(country)
ORDER BY "Customer Amount" desc;
```
From Query 1,2 and 3, knowing the origin of the customer base and its profits generating, staff could act on producing some cultural-related events to promote the stores since they have a clear picture of the target audience.

Query 4: Who are the top 10 customers per total sales? 

Key feature to show is AS. Group by and limit will be used in order to return Customer and Amount. 

```
SELECT first_name AS "First Name", last_name AS "Last Name", SUM(amount) AS "Amount"
FROM customer
JOIN payment on customer.customer_id=payment.customer_id
GROUP BY first_name, last_name
ORDER BY "Amount" desc
LIMIT 10
```
After getting the top 10 customers, rewards could be given and hence developing loyalty programs to retain customers.

## To know about films
Query 5: Who are the top 10 most popular actors on the rank? 

Key feature to show is Inner join. Order by will also be used to return Actors and Rental Rate.
```
SELECT first_name, last_name, (SUM (rental_rate)) AS "Rental Rate"
FROM actor a
JOIN film_actor fc ON a.actor_id=fc.actor_id
JOIN film ON fc.film_id=film.film_id
GROUP BY first_name, last_name
ORDER BY "Rental Rate" desc
Limit 10
```
From the above, some interesting facts are derived from the top 10. The rank could be utilised to draw potential customers' interests.  

Query 6: What are the top 10 films rented? 

Key feature to show is Limit. Order by will be also used to return Films and Rental Rate
```
SELECT title AS "Films"
FROM film
GROUP BY "Films"
ORDER BY SUM(rental_rate) desc
Limit 10
```
From the above, top 10 films that are highly popularized among customers are listed. Staff can hence suggest valid recommendations to customers. 

Query 7: What are the top 3 genres and what are their total sales?

Inner Join will be used. Group by and  in order to return Genres and Total Sales.
```
SELECT name AS "Genres", SUM (amount) AS "Total Sales"
FROM category
JOIN film_category ON category.category_id=film_category.category_id
JOIN film ON film_category.film_id=film.film_id
JOIN inventory ON film.film_id=inventory.film_id
JOIN rental ON inventory.inventory_id=rental.inventory_id
JOIN payment ON rental.customer_id=payment.customer_id
GROUP BY "Genres"
ORDER BY "Total Sales" desc
```
Through joining relevant tables and querying through the sum of the amount, the result shows that "Sports", 
"Animation" and "Action" are the most profit-earning films. 

Query 8: What is the average rental rate for each genre? 

Key feature is to show Average. Inner join and Group by will also be used to return Genre and Average Rental Rate.
```
SELECT name AS "Genres", AVG (rental_rate) AS "Average Rental Rate"
FROM category
JOIN film_category ON category.category_id=film_category.category_id
JOIN film ON film_category.film_id=film.film_id
GROUP BY "Genres"
ORDER BY "Average Rental Rate" desc
```
From the above, after calculating the average rate of rental, it is highlighted that "Games" has the highest average rental rate, in order words it is the most popular Genre among all.  

## To know about stores
Query 9: Which store is making more sales? 

Key feature to show is the Group by to return Store and amount.
```
SELECT store.store_id AS "Store", SUM (payment.amount)
FROM store
JOIN staff ON staff.store_id=store.store_id
JOIN payment ON staff.staff_id=payment.staff_id
GROUP BY "Store"
ORDER BY SUM (payment.amount) desc
```
Through Group by, joining the tables and summing up the payment amount, it is observed that store 2 has a higher sales amount, in order words having a better performance.

Query 10: Which store has higher free rental films rented?

Key feature is to show Count.
```
SELECT store.store_id AS "Store", COUNT (payment.amount=0)
FROM store
JOIN staff ON staff.store_id=store.store_id
FULL JOIN payment ON staff.staff_id=payment.staff_id
GROUP BY store.store_id
ORDER BY store.store_id desc
```
By joining the tables and counting the payment amount equal to 0, it is shown that store 2 has more films full-of-charge rented. 

## Download the PostgreSQL sample database

The above database can be downloaded via the link here: 

https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip

