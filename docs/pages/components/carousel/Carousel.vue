<template>
    <div>
        <div class="content">
            <blockquote>
                Because images can take a few seconds to load (or not at all), use the <code>image</code> container to specify a <strong>precisely sized</strong>
                container so that your layout isn't broken because of image loading or image errors - Bulma <a href="https://bulma.io/documentation/elements/image/" target="_blank">image</a>.
            </blockquote>
        </div>

        <Example :component="ExSimple" :code="ExSimpleCode" paddingless vertical />

        <Example title="Custom" :component="ExFull" :code="ExFullCode" paddingless />

        <Example title="Arrow" :component="ExArrow" :code="ExArrowCode" paddingless />

        <Example title="Progress" :component="ExProgress" :code="ExProgressCode" paddingless />

        <Example title="Indicator" :component="ExIndicator" :code="ExIndicatorCode" paddingless />

        <p class="has-text-centered">Some source by <a href="https://picsum.photos/" target="_blank">Picsum</a> and Images from <a href="https://unsplash.com/" target="_blank">Unsplash</a>.</p><br>

        <Example title="Custom Indicators" :component="ExCustomIndicator" :code="ExCustomIndicatorCode" paddingless>
            When images more than 6 add <code>indicator-custom</code><br>
            If want custom indicator to stay big, use <code>is-medium</code> on <code>indicator-custom-size</code>
        </Example>

        <Example title="Switch like a gallery" :component="ExGallery" :code="ExGalleryCode" paddingless>
            You may also want to add <code>is-clipped</code> modifier to a containing element (usually <code>html</code>) to stop scroll overflow.<br>
        </Example>

        <ApiView :data="api"/>
        <VariablesView :data="variables"/>
    </div>
</template>

<script>
    import api from './api/carousel'
    import variables from './variables/carousel'

    import ExSimple from './examples/ExSimple'
    import ExFull from './examples/ExFull'
    import ExArrow from './examples/ExArrow'
    import ExProgress from './examples/ExProgress'
    import ExIndicator from './examples/ExIndicator'
    import ExCustomIndicator from './examples/ExCustomIndicator'
    import ExGallery from './examples/ExGallery'

    import ExSimpleCode from '!!raw-loader!./examples/ExSimple'
    import ExFullCode from '!!raw-loader!./examples/ExFull'
    import ExArrowCode from '!!raw-loader!./examples/ExArrow'
    import ExProgressCode from '!!raw-loader!./examples/ExProgress'
    import ExIndicatorCode from '!!raw-loader!./examples/ExIndicator'
    import ExCustomIndicatorCode from '!!raw-loader!./examples/ExCustomIndicator'
    import ExGalleryCode from '!!raw-loader!./examples/ExGallery'

    export default {
        data() {
            return {
                api,
                variables,
                ExSimple,
                ExFull,
                ExArrow,
                ExIndicator,
                ExProgress,
                ExCustomIndicator,
                ExGallery,
                ExSimpleCode,
                ExFullCode,
                ExArrowCode,
                ExProgressCode,
                ExIndicatorCode,
                ExCustomIndicatorCode,
                ExGalleryCode
            }
        }
    }
</script>
