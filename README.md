# tableheadfixer
JQuery plugin to fix table header on top when windows scroll hide the head

## Install it via npm
`npm i tableheadfixer`

### Use

    require('tableheadfixer');

    if (typeof $ === "function") {//If jQuery load?     
        if (typeof $.fn.tableHeadFixer === "function") {
            //If table-fixed-header load?
            var container = $(this.$el).find(".page-content");
            $(el).tableHeadFixer({
            container: container,
            beforeTransform: function(val) {
                let th = page.find("thead");
                if (!th.length || val == 0) return val;

                if (!header.hasClass("navbar-hidden")) {
                return val + header.height();
                }
                return val;
            }
            });
        }
    }
